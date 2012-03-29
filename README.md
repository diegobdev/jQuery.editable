jQuery.editable plugin
======================
Editable block element plugin for jQuery

DEMO
----
[http://dev.shokai.org/js/jquery-editable/](http://dev.shokai.org/js/jquery-editable/)

SYNOPSIS
--------

Load jquery.editable.js

    <script src='jquery.js' type='text/javascript'></script>
    <script src='jquery.editable.js' type='text/javascript'></script>


Make editable

    $('span#edit').editable('click', function(e){
      alert(e.value);
    });


Double click

    $('span#edit').editable('dblclick', function(e){
      alert(e.old_value + ' -> ' + e.value);
    });


Edit with Button

    var option = {trigger : $('input.btn_edit'), action : 'click'};
    $('span#edit').editable(option, function(e){
      alert(e.value);
    });