# php-snippets
Collection of PHP Snippets I find useful.

## Sending SMS

While working on web or mobile applications, you often face a situation where you need to send an SMS to your user either for login purposes or providing them with some information. The below PHP function would help you with it.

For sending SMS using any language, you’d need an SMS gateway. Most of the SMS providers these days provide with an API. For the below PHP snippet, I am using MSG91 as SMS gateway.

Syntax:

    <?php
    $message = "Hello World";
    $mobile = "918112998787";
    send_sms($mobile,$message);
    ?>
    
## Get IP Address

get_ip_address -- Retrieves Ip adres from user and checkes for proxy server.

(string) get_ip_address()

This simple function checkes whether the uses is behind a (transparent) proxy, and returns the found IP adres. 

**PHP Call**

    <?php
    echo get_ip_address();
    ?>