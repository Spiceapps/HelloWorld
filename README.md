
# HelloWorld

## Building the website

To make this website i install visual studio on my PC, then added a new web app project, as per the instructions.
i built it, saw that it was working on my PC, and so i published it locally, and then copied over the files over RDP to the windows server.

## Deploying the website

to host it on the IIS, i created a folder under my documents folder, and placed the files there.
then i created the app pool identity, gave it modify permissions on the website folder, and set up the site with it, including the port binding to 5100
**that didn't work.** i found that the "test settings" showed there was a problem with the authorization, despite confirming that the appropriate permissions were set.
in addition, there were errors when trying to access the feature properties. that was solved by installing the "ASP.NET Core 6.0 Runtime" on the server.
