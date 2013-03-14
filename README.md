Written by [Tobias Hourst](tobiashourst@gmail.com)

#SymfonyStartupBoost

## What is it?

To save time when starting a new project with Symfony2, `SymfonyStartupBoost` contains a couple of pre-configured empty repositories with the ``Acme namespace`` **removed**.

Go through the different master branches to find one that suits your needs.

			Notes: 
			--------------
			- None the builds use *Assetic* to load *CSS* files. 
			- Make sure you understand all requirements each build require.

Here are some example of builds:
	
	**With front-end librairies:**
	
	- Symfony2 v2.2.0 + Zurb Foundation 4.0.5 *(with SASS)* +  Compass.
	- Symfony2 v2.2.0 + Zurb Foundation 4.0.5 *(without SASS)*.
	- Symfony2 v2.2.0 + MopaBootstrapBundle *(Twitter Bootstrap)* + Compass.
	- Symfony2 v2.2.0 + MopaBootstrapBundle *(Twitter Bootstrap)*.
	
	**With front-end & back-end librairies:**
	
	- Symfony2 v2.2.0 + Zurb Foundation 4.0.5 *(with SASS)* +  Compass **/** FOSUserbundle + KNPMenuBundle.
	- Symfony2 v2.2.0 + Zurb Foundation 4.0.5 *(without SASS)* **/** FOSUserbundle + KNPMenuBundle.
	- Symfony2 v2.2.0 + MopaBootstrapBundle *(Twitter Bootstrap* + Compass **/** FOSUserbundle + KNPMenuBundle.
	- Symfony2 v2.2.0 + MopaBootstrapBundle *(Twitter Bootstrap)* **/** FOSUserbundle + KNPMenuBundle.
	
## HowTo Get Started

### Clone the Branch you Picked up:

```bash
 $ git clone git@github.com:tobyhourst/SymfonyStartupBoost.git -b branch_name /path/to/download/location
```
**Note:** replace ``branch_name`` & ``/path/to/your/local/server`` appropriately.


### Little Configuration

- Rename the downloaded folder to ``your_project_name``
- Install the vendors:

```bash
 $ cd /path/to/folder
 
 # if composer is globally installed on your machine, run:
 $ composer install
 
 # or else, get composer executable:
 $ curl -sS https://getcomposer.org/installer | php
 # then install the vendors:
 $ php composer.phar install 
```

- Make sure ``app/cache`` and ``app/logs`` have the right permissions:

```bash
 $ (sudo) chmod 777 app/cache app/logs
```

- Point to: ``http://localhost/your_project_name/app/check.php`` to make sure your server meets all Symfony2 requirements.

### Start Developing

- Point to: ``http://localhost/your_project_name/web/`` for a warm welcome page.
