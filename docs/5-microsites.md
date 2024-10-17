---
id: microsites
title: Microsites module
---

# Microsites module.

You can enter the module dedicated of microsites management doing click in the 
framing option for left side bar.<br/>
![Texto alternativo](/docs_img/microsites_dash.png "User panel")

# SUPER ADMIN.

Like an admin you can see the following options and they will be explained in 
the order image.
![Texto alternativo](/docs_img/microsites_panel.png "User panel")

## See all microsites.

Can see all microsites inmediatly enter to the module and they are separated by his site type.

## Create new microsite.

You can create a new microsite doing click in the button "Create microsite" and will be 
redirect to the create microsite form.
![Texto alternativo](/docs_img/create_microsite_form.png "User panel")

* Fields
    * [Slug](#slug)
    * [Expiration time](#expiration-time)
    * [Site type](#site-type)
    * [Logo](#logo)


### Slug.

The slug is a whitout spaces name for identify the site like unique.

### Expiration time.

When the peyer go to made a pay, this session have the expiration time for default in
the site, this time is established here and you need to enter a time in minutes, you can
use minum ten minutes and maximun 30 minutes.

### Site type.

Can select for a new site one of three types of sites:

  * Donations:
        These are a sites for pay a free amount, the payer can decide the value for pay and 
        his input these value, is used communtly for a donations.

 * Invoices:
        These are a sites for upload invoices and the payer just can pay the invoice associated 
        whit his and can't modify the value.

 * Suscription:
        These are a sites for offer a product/service to user through a plan, the plan have a value,
        expiration time and the user can cancell in any moment and hace automatic debits.

### Logo.

Can add a logotype for site, the name need to be without spaces and extension ".jpg" - ".png" - ".jpeg" 
and have a limit weight above 2048mb.

## Actions.

* Actions
    * [Eye-button](#eye-button)
    * [Pencil-button](#pencil-button)
    * [Trash-button](#trash-button)
    * [Bars-button](#bars-button)
    * [Magnifying glass-button](#magnifying-glass-button)
    * [Select file-button](#select-file-button)


### Eye-button.

In the actions when you click the eye-button you can see the full information 
for the respective microsite and if you click the pencil-button you can edit this microsite.<br/>
![Texto alternativo](/docs_img/see_site_form.png "User panel")

### Pencil-button.

You can edit a microsite doing click in the pencil-button located in these specific microsite form or in the 
main microsite page.
![Texto alternativo](/docs_img/edit_site_form.png "User panel")<br/>
If you don't change the logo, these will be the same when the site are modify.

### Trash-button.

You can delete a site press the trash-button if you are Super Admin - Admin user.

### Bars-button.

In this sub-module you can like and Super Admin - Admin user modify the fields will be requested for the payer 
at the moment to made a pay, for default in the site are a locale and total information to be request for the
donations and suscriptions sites, for the invoices sites, the currency are default too but for create a invoice
with these specifics currencies.
![Texto alternativo](/docs_img/manage_site_fields.png "User panel")<br/>
When you press the plus-button for a fields to add you can see the following configuration for his field:

* Configuration
    * [Field-type](#field-type)
    * [Is optional?](#is-optional)
    * [Is modify?](#is-modify)
    * [Values for this field](#values-for-this-field)

#### Field-type.

Can select between "Text", "Number" or "Select" options for the field.

#### Is optional?

You decide if the field are can optional for the payer or you will establishes a default value, if the payer not 
fill this field, the pay session execute correctly.

#### Is modify?

You decide if the field are can modified for the payer or you will establishes a default value, if the payer not 
fill this field, the pay session not will be execute.

#### Values for this field.

If the field is "Select type", "Not optional" and/or not modify you need to establish a default value for the payer
can decide or the pay session will be executed correctly.

For the "Select type", the values are separated by comma(,).

When you finalice press button "Add field" and you can see in the table at the bottom with the information suministrated.

**Note:**
Can delete all fields except the default fields clicking the tras-button in the actions column for the avalible fields.

### Magnifying glass-button.

When press this button can see all the pays maded associated with this site.

### Select file-button.

When you press this button the picker file for youre system will be opened for can select a Excel file with the extension 
.xlsx only and the invoices content in his file are saved in the database, the file need to be needed structure for the 
correct work of the import masive invoices.
