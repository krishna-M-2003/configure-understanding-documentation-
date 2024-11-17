## Configuration understanding document

## Topics

### Apps 
### Connector 
### Collection ,Entity 
### SingleEntity
### Field,
### FieldGroup
### Form - Basics Of All Type
### Datasource
### Viewoptions Configuration
### Page - widgtes
### Action, Activity

* Goto the url [https://apps4x.web.app/](https://apps4x.web.app/)

* We must first log into the apps4x.web.app.

* It will take you to the Organization page after you log in. 

* Now you can create a organization with pro options 

* what is pro option ?
    
   In addition to other options, it has complete access to configure the apps.

* click the Home icon in your organization.    

* You'll see that the Home already has the studio app installed. 

* The default studio app was made by the app itself when we create the organization.

* create a new app by click the app + button.

* We add the configuration to the app we made after finishing all the setup in the studio app. 

*  It is necessary to have a connection ID in order to construct collections.

* Go back to the URL [https://apps4x.web.app/#/LGE0000006/Studio](https://apps4x.web.app/#/LGE0000006/Studio).

* The **Connectors** menu is visible at the top.

* Click the Add icon after selecting the connectors. 

* A popup window will open; fill in the required fields for Name, Image, and ConnectorType.Choose _SQL_ as the connector type. 

* Click on the app that you made at the stating stage in the studio. We now noticed a **_collections_** menu. After selecting the + icon in the collection and selecting _add collection_, a popup window appeared with some fields to fill out. Once the forms were filled out, the collection had been created.

* what is collection ?
   
  A group of entities or an entity's parent is called a collection.

* There are three tabs in the collection: _Type_, _Fields_, and _Forms_. 

  * The type in the collection contains the following entity's.

   Example:

    _**Help Content**_ is a collection.

     The following entities are found in the **Help Content** collection: "Guide, FAQ,  Help category".

  * Field tab - Create the field what we desire.

  * Form 

* To create an entity, choose the **add entity** option that appears when you click on the collection you created. 

* _notes:_ There are several entities in the collection. 

* Create an entity field; the creation of an entity field depends on the data in the collection field.

* Basic Forms Types -
   
   * Table - its has **Configurtion** like show edit or not show create or not like that, **Colomns** add the wanted colonms, **Datasource** select what your need like Rest Api, Collection, entity, ect.. **sorting**
  
   * CustomTemplate - its has HTML, CSS, JS, Configuration 
   * Details - design, rules, config

* Then add page, click the add button on the bottom it open the page widgtes and select any one of them (entity, tab, custom template) and fill the fields and click save.

### Action

* Action in configuration can mean several different things. Clicking on a button is one of the fundamental meanings, and other activities are referred to as actions.

* Data from one Entity Table Form is transferred to another using this action, which also displays the data on the Details Page when the Action Button is clicked.

### Who to create and use the Action :

* We start by clicking the __Studio__.
* After selecting the collection, select the entity.
* The *Action* menu will appear on the page.
* Clicking the __Create__ button will let you create an action.
* It will Create with the following Fields
  * Id
  * Name
  * Status
  * Version
  * Action

* After clicking the ID, the Action Form page will be redirected. Next, configure the field that you wish to see in the Action form.

* Go to the app and select the __Option__ menu, which appears at the top of the table.

* Click the Option ->More Options -> Scroll down to find the Add Column.

* Click Create ClientField, then add *lable*, *Name*, and *Datatype*. And submit it.

* What you created in the ClientField it visible in the Columns click the settings on the created columns. On the View Option page, the setting is located on the right side.

*  A **Form Config** popup will open then select the **Viwe type** in to **Button**, **Button Type** into **Option Action**, and select the **Action Form** in to Action we created in the entity then Submit it.

* Then goto __Data Source__ in the __View Option__ page select the __Datasource Type__ in to __Entity__, select __Entity List__ into you Entity name, select __Action type__ into *create, updata, delete* based on you needs and purpose.

* Field value:
  * If you want the table data you will use the __params__.

    Ex: you want Table data - __{{ params.value }}__.

  * If you want the form data you will use the __FormData__.

    Ex: you want Form data - __{{ FormData.value }}__.

### Activity		

 Although it has a slight modification on the details page, __Activity__ functions similarly to __Action__.

 * On the details page, the __Action__ is at the top and the __Activity__ is at the bottom.
