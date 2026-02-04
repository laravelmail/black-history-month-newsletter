# Black History Month Newsletter

Professional Black History Month Newsletter celebrating achievements and contributions of African Americans across various industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Media, Education
- **Message Type:** Newsletter
- **Tags:** blackhistorymonth, culturalawareness, diversity

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/black-history-month-newsletter.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/black-history-month-newsletter/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.black-history-month-newsletter',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
