#Log-ins
Adding log-ins/authentication to a service is a larger undertaking than it looks.

##Guidance/Tool
Don't. Building a login system is a significant undertaking. While there are numerous open source libraries that make it trivial to add login functionality to your service, the moment you add that feature you're significantly increasing your user support overhead (people forget how to sign in, lose their passwords, etc), you're accruing personal data that you will need to constantly review and protect, and you're adding a relatively complex interaction for users to complete.

Many features that are often implemented using login systems can be completed in other (and potentially more useful) ways. Saving search results, for example, doesn't require a login but just a way of helping users remember a specific URL. Instead of having them log in you could provide a tool to help send the URL to an email address or instructions on creating a bookmark in their browser. Or perhaps you could just take their email address and let them know if the search results change? The precise details will vary according to what users need from your service, but if there's an alternative to a login system that should be preferred.

If after careful review and design work there is no option but to build a login system you should talk to the GDS ID Assurance team.

##Code/Templates
If you're giving people code r copy to cuta and paste then here is where it will go.

##Why we do this
This is the reasoning for the decision. You might want to link to relevant blog posts or legislation here.

##Further reading
Link within the Manual, or to other posts, that will help people to work on the tool.