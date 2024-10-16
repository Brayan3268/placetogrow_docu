---
id: invoices
title: Invoices module
---

# Invoices module.

You can enter the module dedicated of invoices management doing click in the 
framing option for left side bar.<br/>
![Texto alternativo](/docs_img/invoices_dash.png "User panel")

# SUPER ADMIN.

Like an admin you can see the following options and they will be explained in 
the order image.
![Texto alternativo](/docs_img/invoices_panel.png "User panel")

## See all invoices.

Can see all invoices inmediatly enter to the module and can see the main information
for each invoice and can filter for each column and do filter combinates.

### Navigate invoices.

You can navigate for the users and sites if you click the hyperlink on the 'User's document' and 'Site' columns.

## Create new invoice.

You can create a new invoice doing click in the button "Create new invoice" and will be 
redirect to the create invoice form.
![Texto alternativo](/docs_img/create_invoice_form.png "User panel")

* Fields
    * [Reference](#reference)
    * [Amount to request](#amount-to-request)
    * [Currency](#currency)
    * [User](#user)
    * [Site](#site)
    * [Invoice surcharge](#invoice-surcharge)
    * [Surcharge for invoice](#surcharge-for-invoice)
    * [Date expiration](#date-expiration)


### Reference.

The reference need to be unique for this site and can be alphanumeric.

### Amount to request.

This is the value to pay by the payer.

### Currency.

This is the currency asociated to the amount for pay.

### User.

In this fiel is completly needed to select the document of the user, the app only 
permmit asociate invoices to guest users.

### Site.

In this fiel is completly needed to select the site to will be associated to the invoice, 
the app only permmit asociate invoices to invoices sites.

### Invoice surcharge.

This is the date for apply to the ***Amount to request*** value the ***Surcharge for invoice*** value.

### Surcharge for invoice.

This is the amount to add at the "Amount to request" if the invoices not was payed after the 
invoice surcharge date.

This value can be a numeric value or a percentage value, see the next example.

 **Numeric value:** If the ***Amount to request*** are: $10.000 and the ***Surcharge for invoice*** are
$5.000, once time the ***Invoice surcharge*** date is reached, the ***Amount to request*** value will be: 
$15.000, these value are the add between ***Amount to request***($10.000) and ***Surcharge for invoice***
($5.000).

 **Percentage value:** If the ***Amount to request*** are: $10.000 and the ***Surcharge for invoice*** are
 50%, once time the ***Invoice surcharge*** date is reached, the ***Amount to request*** value will be: 
$15.000, these value are the add between ***Amount to request***($10.000) and the 50% from ***Amount to request***($10.000).

***Note:*** The percentage value must be a number between 0 and 100 and must to be followed for a '%' sign.

### Date expiration.

This is the date for made unavalible to pay the invoice, because the invoice with this state not to be show for the users.

## Actions.

* Actions
    * [Eye-button](#eye-button)
    * [Pencil-button](#pencil-button)
    * [Trash-button](#trash-button)


### Eye-button.

In the actions when you click the eye-button you can see the full information 
for the respective invoice and if you click the pencil-button you can edit this invoice.<br/>
![Texto alternativo](/docs_img/see_invoice_form.png "User panel")

### Pencil-button.

You can edit a invoice doing click in the pencil-button located in these specific invoice form or in the 
main invoice page.
![Texto alternativo](/docs_img/edit_invoice_form.png "User panel")<br/>

### Trash-button.

You can delete a invoice press the trash-button if you are Super Admin - Admin user.

## Masive upload invoices.

In the app, can upload a masive number of invoices in the site module with an Excel document, these excel
need to have the following structure:<br/>
![Texto alternativo](/docs_img/excel_structure_invoice.png "User panel")<br/>

### Column A:

In this column need to enter the invoice reference.

### Column B:

In this column are allowed the ***Amount to request*** value, it's mean, the valu to will be payed.

### Column C:

In this column goes the denomination of the payment. 

### Column D:

In this column goes the user document for can asociated the invoice with a user.

### Column E:

In this column goes the date for create a invoice, ussualy are the current day.

### Column F:

In this column goes the ***Surcharge for invoice*** date.

### Column G:

In this column goes the ***Surcharge for invoice*** to will be added to ***Amount to request*** according the
behavior page.

### Column H:

In this column goes the date for expired a invoice and are the unavalible to pay for the user.

## Invoice status

The invoice can get the following status:<br/>
![Texto alternativo](/docs_img/invoices_status.png "User panel")<br/>

### not_payed:

This is the default state for a invoice when is created and haven't interaction.

### payed:

This is the state when invoice getting payed.

### expirated:

This is the state when invoice not be payed and the ***Date expiration*** is reached.

### pending:

This is the state when the invoice pay's is pending and can't get a different state in the main session.

### unknow:

This is a default state for a uncatched error in the invoice pay's.