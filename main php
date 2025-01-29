<?php
/**
 * Plugin Name: WooCommerce Hide Order Notes
 * Plugin URI: https://www.bedrukt.nl
 * Description: WooCommerce Hide Order Notes verbergt het notitie veld bij de checkout.
 * Version: 1.0.0
 * Author: J.P. van der Meer
 * Author URI: https://www.bedrukt.nl
 * License: GPL2
 * WC requires at least: 3.3
 * WC tested up to: 4.7.0
 */

// Removes Order Notes Title - Additional Information & Notes Field
add_filter( 'woocommerce_enable_order_notes_field', '__return_false', 9999 );



// Remove Order Notes Field
add_filter( 'woocommerce_checkout_fields' , 'remove_order_notes' );

function remove_order_notes( $fields ) {
     unset($fields['order']['order_comments']);
     return $fields;
}
