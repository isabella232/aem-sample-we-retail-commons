# We.Retail Commons

This is the We.Retail Commons project.

## Modules

The main parts of the template are:

* ui.content: contains product data and assets

## How to build

To build all the modules run in the project root directory the following command with Maven 3:

    mvn clean install

If you have a running AEM instance you can build and package the whole project and deploy into AEM with  

    mvn clean install -PautoInstallPackage
    
Or to deploy it to a publish instance, run

    mvn clean install -PautoInstallPackagePublish

## Maven settings

The project comes with the auto-public repository configured. To setup the repository in your Maven settings, refer to:

    http://helpx.adobe.com/experience-manager/kb/SetUpTheAdobeMavenRepository.html

## Releasing

In order to release this package and distribute it to https://bintray.com/adobe-marketing-cloud/aem-samples/we.retail.commons/0.2.0, you must add the following to your Maven `settings.xml` file (`~/.m2/settings.xml`):

    <server>
        <id>bintray</id>
        <username>BINTRAYUSERNAME</username>
        <password>BINTRAYPASSWORD or APIKEY</password>
    </server>