# jQuery

    $('.myClass').find('input').each(function() {
        /* CODE HERE */
    });


# PURE JS

    let myClass = document.querySelectorAll('.myClass');
    myClass.forEach(function (myClassEl, index) {
        let find_input = myClassEl.querySelectorAll('input');
        find_input.forEach(function (find_inputEl, index) {
            /* CODE HERE */
        });
    });
    
    
