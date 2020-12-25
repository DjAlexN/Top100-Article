# Top100-Article
The module displays the top 100 best articles displayed by the number of comments, number of views and number of ratings

# Instrukcja po Polsku
1. W folderze "templates" zmień nazwę folderu "{THEME}" na nazwę swojego szablonu jai używasz na stronie
2. Wgraj foldery: "engine" oraz "templates" na swój serwer.
3. W Panelu Administratora w sekcji Zarządzania Wtyczami wgraj plik top100news.xml
4. W swoim szablonie w wybranym miejscu (np w pliku main.tpl) dodaj odnośnik do podstrony która wyświetla ostatnio edytowane artykuły.

Odnośniki:
http://twoja-strona.pl/?do=top100&mode=rating 
http://twoja-strona.pl/?do=top100&mode=comments 
http://twoja-strona.pl/?do=top100&mode=views 
Lub:
http://twoja-strona.pl/top100/rating 
http://twoja-strona.pl/top100/comments 
http://twoja-strona.pl/top100/views 

5. W głównym pliku .htaccess na serwerze znajdź linijkę: 

RewriteEngine On

Poniżej dodaj:

RewriteRule ^top100/([^/]*)(/?)+$ index.php?do=top100&mode=$1 [L]

6. Gotowe :) Teraz możesz cieszyć się modułem

# English manual
1. In the "templates" folder change the name of the "{THEME}" folder to the name of your template you use on the website
2. Upload the folders: "engine" and "templates" to your server.
3. In the Administrator Panel, in the Plugins Management section, upload the top100news.xml file
4. In your template, in the selected place (eg in the main.tpl file) add a link to the subpage that displays recently edited articles.

Reference:
http://twoja-strona.pl/?do=top100&mode=rating 
http://twoja-strona.pl/?do=top100&mode=comments 
http://twoja-strona.pl/?do=top100&mode=views 
or:
http://twoja-strona.pl/top100/rating 
http://twoja-strona.pl/top100/comments 
http://twoja-strona.pl/top100/views

5. In the main .htaccess file on the server, look for the line:

RewriteEngine On

Add below:

RewriteRule ^top100/([^/]*)(/?)+$ index.php?do=top100&mode=$1 [L]

6. Done :) Now you can enjoy the module
