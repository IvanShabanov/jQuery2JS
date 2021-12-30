# ATTRIBUTES


# jQuery

    let type = $(".my_class").attr("type");
    $(".my_class").attr("type", "newtype");
    $(".my_class").removeAttr("type");
    
    
# PURE JS

    let type = document.querySelector(".my_class").getAttribute("type");
    document.querySelector(".my_class").setAttribute("type", "newtype");
    document.querySelector(".my_class").removeAttribute("type");


#ALSO

    /* All Attributes */
    let allAttributes = document.querySelector(".my_class").attributes;
    for (let attr of allAttributes) {
        alert( `${attr.name} = ${attr.value}` );
    };
    
    /* Check attribute exists */
    let type = 'empty';
    if (document.querySelector(".my_class").hasAttribute("type")) {
        type = document.querySelector(".my_class").getAttribute("type");
    };
