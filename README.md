templatehelperz
===============

Drupal - Module: templatehelperz

Usage:

$template_var = field2var( $vars_temp, $node );

$vars_temp = array(
    'type' => '',             //image, images, term, text, list, ingrediente, vimeo_embed, vimeo_url
    'field' => '',            //name of the field (field_image, field_tags, ...)
    'style' => array(
      'preset' => '',         //name of the image style (200x100, 366x133, ...)
      'width' => '',          //width
      'height' => '',         //height
    ),
    'class' => '',            //class for each element (default: none)
    'no_container' => false,  //the container that holds all the elements (default: tag -> ul, class -> galerie clearfix)
    'container' => array(
      'tag' => '',            //DOM tag for the container (default: ul)
      'class' => '',          //class for the container ( default: galerie clearfix)
    ),
    'no_wrapper' => false,    //the wrapper for each element (default: tag -> li, class -> item)
    'wrapper' => array(
      'tag' => '',            //DOM tag for the wrapper of each element (default: li)
      'class' => '',          //class for the wrapper of each element (default: item)
    ),
    'og' => false,            //set the og:image meta tag in the head
    'link_to' => array(
      'href' => '',           //link tag for each element to link to a specified url (include http://)
      'rel' => '',            //rel attribute for the link tag
      'target' => '',         //target attribute for the link tag
      'style' => '',          //link tag for each element to link to a specified image preset style (200x100, 366x133, full, ...)
    ),
    'separator' => array(
      'value' => '',          //separator char for terms (default: none)
      'tag' => '',            //separator wrapper DOM tag (default: li)
      'class' => '',          //separator wrapper class (default: separator, class item is added each time)
    ),
    'label' => array(
      'value' => '',          //adds an element at the begining of the list with the set value (default: none)
      'tag' => '',
      'class' => ''
    ),
    'properties' => array(
      'name' => 'value'       //adds custom properties to the item
    )
  );  