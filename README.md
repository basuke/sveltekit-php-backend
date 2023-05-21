# PHP Backend for SvelteKit

You can have PHP logic directly in SvelteKit route directory like this: `+page.server.php`

```PHP
<?php
function load($event) {
    $name = ($event->params['name'] ?? 'unknownn');
    return [
        'message' => "Hello " . $name,
    ];
}
```

## Installation

See https://github.com/basuke/vite-plugin-sveltekit-php-backend

## License

MIT
