# Events

Flare includes a number of Events which you can listen for when implementing
custom Admin functionality. 

For instance you might wish to send out a push notification when a certain 
Model type has a new record created. This can be acheived by creating a listener
class and registering it in your `EventServiceProvider` bound to the Flare
event.

## Model Events

### Create

### Edit

### Save

### Delete & Soft Delete

### View

### Custom Events

All Event classes extend the abstract `ModelAdminEvent` which has a property
of `$modelAdmin` with the `\LaravelFlare\Flare\Admin\Models\ModelAdmin` 
instance. 

You can create your own classes which extend `ModelAdminEvent` which can be as
simple as:

```php

<?php

namespace App\Events;

use LaravelFlare\Flare\Events\ModelAdminEvent;

class ModelCloned extends ModelAdminEvent
{
}
```

This event can then be fired in your custom Admin code (such as a 
`ModelAdminController`) with the following:
```php
event(new ModelCloned($modelAdmin));
```