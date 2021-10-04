
# POST DATA 


# jQuery

    $.ajax({
        type: "POST",
        url: "/targeturl/",
        data: data,
        success: function (result)
        {
            /* ANALIZE result */
        }
    });
    
    
# PURE JS

     fetch("/targeturl/", {
        method: 'POST',
        body: data,
    }).then(function (response) {
        return response.text(); /* to get HTML */
        //return response.json(); /* to get JSON */
    }).then(function (result) {
        
        console.log(result); 
        
        /* Convert result to HTML DOM*/
        let parser = new DOMParser();
        let resultDom = parser.parseFromString(result, 'text/html');
         
        /* ANALIZE resultDom*/

    })
    .catch(function (err) {
        console.log('Something went wrong. ', err);
    });
