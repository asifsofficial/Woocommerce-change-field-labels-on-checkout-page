# Woocommerce-change-field-labels-on-checkout-page


## Location:
```
functions.php
```
```
 add_filter( 'woocommerce_default_address_fields' , 'wc_rename_state_province', 9999 );

function wc_rename_state_province( $fields ) {

    $fields['country']['label'] = 'Country';
    $fields['first_name']['label'] = 'Your First Name';
    $fields['last_name']['label'] = 'Your Last Name';
    $fields['address_1']['label'] = 'Addess';
    $fields['state']['label'] = 'City';
    return $fields;

}
```
