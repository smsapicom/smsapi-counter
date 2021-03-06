# Script that helps to count number of characters in message and how many parts SMS will contain.

## Usage

You should add **smsapi-counter.js** or **smsapi-counter.min.js** files at the end of `<body>` element. You can find an example in **demo.html** file.

### HTML

Activate counter with specified attributes. You have to target `<textarea>` and one random element (`span`, `h1`, `h2` etc) to show current characters count. With HTML you can activate one counter per page. To include more text areas with counters, use JavaScript activation method.

```html
    <textarea data-cv-sms-textarea></textarea>
    <span data-cv-sms-counter></span>
```

### Javascript

After loading smsapi-counter JavaScript file, use this method. You have to specify two parameters: ID of `<textarea>`, and ID of label that will show current characters count.

```javascript
    CVSMSCounter.activate('textareaID', 'counterLabelID');
```

## WARNING!
We reccomend to use UTF-8 encoding. **Script might count characters wrong if you will use wrong encoding or message is filled using copy/paste method**. If you want to protect additionally you can use parameters like ***nounicode***, ***normalize***, ***max_parts***. You can find more details about parameters in [SMSAPI.com specification](https://www.smsapi.com/rest).