# Script which helps you to count number of characters in entered message and how many parts will SMS contain.

## Usage

You should add **smsapi-counter.js** or **smsapi-counter.min.js** files ad the end of `<body>` element. You can find example in **demo.html** file.

### HTML

Activate counter with specified attributes. You have to target `<textarea>` and one random element (`span`, `h1`, `h2` etc) to show current characters count. With HTML you can activate one counter per page. To include more textareas with counters, use javascript activation method.

```html
    <textarea data-cv-sms-textarea></textarea>
    <span data-cv-sms-counter></span>
```

### Javascript

After loading smsapi-counter javascript file, use this method. You have to specify two parameters: ID of `<textarea>`, and ID of label that will show current characters count.

```javascript
    CVSMSCounter.activate('textareaID', 'counterLabelID');
```

## WARNING!
We reccomend to use UTF-8 encoding. **Script might count characters wrong if you will use wrong encoding or message is filled using copy/paste method**. If you want to protect additionaly you can use parameters like ***nounicode***, ***normalize***, ***max_parts***. You can find more details about parameters in [SMSAPI.com specification](https://www.smsapi.com/rest).