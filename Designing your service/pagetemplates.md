# Page templates

All pages on GOV.UK need to feel like they're part of the same service.
In particular, the header and footer of every page should be consistent.
This guide explains how to do this.

## The template code

The most up-to-date version of the template code can be found in our ['Static' repository on GitHub](https://github.com/alphagov/static/tree/master/app/views/root). The [_base.html.erb](https://github.com/alphagov/static/blob/master/app/views/root/_base.html.erb) file contains the default template code.

GOV.UK page templates are written in [ERB format](http://ruby-doc.org/stdlib-1.9.3/libdoc/erb/rdoc/ERB.html), but can be easily converted back to plain HTML.

## Template assets

The template code contains absolute links to CSS and JavaScript on our 'assets' subdomain. We recomend that you continue to reference these assets in this way as you develop your service, as opposed to linking to your own copies of these files. That way, you'll always be using the latest version of the assets and you can address any conflicts as and when they arise.

Once the service is ready for production we'll need to decide whether you should continue to link to the assets in this way or whether you should now use your own copies of them. Please contact the GDS team to discuss this at the appropriate time.

## Keeping template code and assets up-to-date

GOV.UK is continuously being improved, which means that template and asset code changes regularly. All services on GOV.UK are expected to keep their templates and assets up-to-date. How you do this will depend on how you implement the templates and where your service is hosted. Please contact the GDS team to discuss options.

## Template elements

### The site header

This is the black strip across the top of every page on GOV.UK.
It contains the GOV.UK logo and the search box.
Please don't add any other elements to the site header.
This element is mandatory.

#### The GOV.UK logo

This must always link back to the [GOV.UK home page](http://gov.uk).

#### The search box

In most cases the default action for the search box should be to perform a search on the whole of GOV.UK.
If your service is to be hosted in the same environment as GOV.UK the default template code will do this.
If your service is to be hosted in a different environment you'll need to change the action attribute of the form as follows: `action="http://gov.uk/search"`.

In some cases we might decide that the scope of the search should be reduced to just pages from your service. In these cases the scope should be clearly indicated in the placeholder attribute and label of the search box.

In order for pages from your service to appear within GOV.UK search results they will need to be indexed. It doesn't always make sense to do this. For example, there's no point indexing a page that can only be reached via a login or as part of a transaction. If we decide that your pages *should* be indexed you'll need to contact the GDS team to discuss the best way of going about this.

### Breadcrumb navigation

This appears immediately below the site header.
All content pages on GOV.UK are given a category and subcategory. These are used to create category pages and breadcrumb navigation. Breadcrumb navigation allows people to broaden their search for information from a specific page to all pages within the same category or subcategory. It also helps them to orientate themselves within the website.

This element is optional. Not all pages require breadcrumb navigation. It depends if the actions that it supports are genuine use cases for a specific page. For example, a page that's part-way through a multi-page transaction would not benefit from breadcrumbs because the user's main goal is completing the transaction, not browsing similar content.

### The main content area

This is where all the page content lives.
All content within this area should be sympathetic to the GOV.UK visual style and use the available design patterns where possible.

There are two main variants of this element: A narrower version with a 'related links' panel on the right, for content pages, and a wider version without a panel for transaction and landing pages.

### The page footer

This is the grey panel at the bottom of every page.
It contains global site navigation and a copyright message.
Please don't add any other elements to the footer.
This element is mandatory.

From time to time we may update the links in the footer. It's important that your web pages are updated promptly when this happens. Contact the GDS team to discuss the best way of ensuring that this happens.