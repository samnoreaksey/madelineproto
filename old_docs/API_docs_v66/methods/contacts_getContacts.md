---
title: contacts.getContacts
description: contacts.getContacts parameters, return type and example
---
## Method: contacts.getContacts  
[Back to methods index](index.md)


### Parameters:

| Name     |    Type       | Required |
|----------|:-------------:|---------:|
|hash|[string](../types/string.md) | Yes|


### Return type: [contacts\_Contacts](../types/contacts_Contacts.md)

### Example:


```
$MadelineProto = new \danog\MadelineProto\API();
if (isset($token)) { // Login as a bot
    $MadelineProto->bot_login($token);
}
if (isset($number)) { // Login as a user
    $sentCode = $MadelineProto->phone_login($number);
    echo 'Enter the code you received: ';
    $code = '';
    for ($x = 0; $x < $sentCode['type']['length']; $x++) {
        $code .= fgetc(STDIN);
    }
    $MadelineProto->complete_phone_login($code);
}

$contacts_Contacts = $MadelineProto->contacts->getContacts(['hash' => string, ]);
```

Or, if you're into Lua:

```
contacts_Contacts = contacts.getContacts({hash=string, })
```
