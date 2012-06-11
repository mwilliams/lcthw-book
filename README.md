Text versions of c.learncodethehardway.org

Generated with the following:

    wget -m -k -e robots=off c.learncodethehardway.org
    for html in *.html
    do
        txt=$(echo $html | sed 's/html$/txt/')
        lynx -dump -nolist $html > $txt && rm $html
    done

