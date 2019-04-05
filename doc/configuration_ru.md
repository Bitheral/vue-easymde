## Конфигурация

- **autoDownloadFontAwesome**: Если стоит значение `true`, принудительно загружает Font Awesome (используется для иконок). Если установлено `false` - предотвращает загрузку. По умолчанию стоит значение `undefined` и будет проверяться, добавлен ли уже Font Awesome, а затем загружать по необходимости.
- **autofocus**: Если стоит значение `true`, автофокусирует редактор. По умолчанию `false`.
- **autosave**: *Сохраняет написанный текст и сможет загружать его в будущем. Текст забудется при подтверждении формы, в которой он содержался.*
  - **enabled**: Если стоит значение `true`, автосохраняет текст. По умолчанию `false`.
  - **delay**: Задержка между сохранениями в миллисекундах. По умолчанию значение `10000` (10сек).
  - **uniqueId**: Чтобы EasyMDE мог использовать автосохранение, нужно настроить строку уникального индентефикатора. Что-то, что отделяет от других настроек EasyMDE на вашем веб-сайте.
- **blockStyles**: Настроить поведение определенных кнопок, меняющих стиль блоков текста.
  - **bold**: Может быть установлено `**` или `__`. По умолчанию `**`.
  - **code**: Может быть установлено ```` ``` ```` или `~~~`.  По умолчанию ```` ``` ````.
  - **italic**: Может быть установлено `*` или `_`. По умолчанию `*`.
- **element**: Элемент DOM для текстовой области. По умолчанию первая текстовая область на странице.
- **forceSync**: Если стоит значение `true`, принудительно сохраняет изменения текста, сделанные в EasyMDE, в исходной текстовой области. По умолчанию `false`.
- **hideIcons**: Массив имен иконок для скрытия. Может быть использован для того, чтобы скрыть некоторые иконки, показанные по умолчанию без полной настройки панели инструментов.
- **indentWithTabs**: Если стоит значение `false`, в отступах используются пробелы вместо табуляции. По умолчанию `true`.
- **initialValue**: Если установлено, то будет задано начальное значение редактора.
- **insertTexts**: Устанавливает поведение определенных кнопок вставки текста. Использует массив с двумя элементами. Первый элемент - текст, который будет добавлен перед курсором или выделением, второй элемент будет вставлен после. Например,  For example, значение ссылки по умолчанию: `["[", "](http://)"]`.
  - horizontalRule
  - image
  - link
  - table
- **lineWrapping**: Если стоит значение `false`, отключить перенос строки. По умолчанию `true`.
- **minHeight**: Устанавливает минимальную высоту для области редактирования до ее авто-увеличения. Должно быть строкой, содержащей подходящее значение CSS, например `"500px"`. По умолчанию `"300px"`.
- **onToggleFullScreen**: Функция, которая вызывается, когда включается полноэкранный режим редактора. Функция будет передана как логическое значение в качестве параметра, `true`, когда редактор переходит в полноэкранный режим, или `false`.
- **parsingConfig**: Настройте параметры для парсинга Markdown во время редактирования (без предварительного просмотра).
  - **allowAtxHeaderWithoutSpace**: Если стоит значение `true`, будут отображаться заголовки без пробела после `#`. По умолчанию `false`.
  - **strikethrough**: Если стоит значение `false`, не будет обрабатываться зачеркнутый синтаксис GFM. По умолчанию `true`.
  - **underscoresBreakWords**: Если стоит значение `true`, слова будут разделяться подчеркиваниями. По умолчанию `false`.
- **placeholder**: Если установлено, то отображается специальное сообщение в поле.
- **previewRender**: Пользовательская функция для парсинга открытого текста Markdown и возврата HTML. Используется при предварительном просмотре пользователем.
- **promptURLs**: Если стоит значение `true`, будет появляться окно предупреждения JS с запросом ссылки или URL-адреса изображения. По умолчанию `false`.
- **promptTexts**: Настройте текст, используемый для запроса URL-адресов.
  - **image**: Текст, используемый при запросе URL изображения.  По умолчанию `URL of the image:`.
  - **link**: Текст, используемый при запросе URL-адреса ссылки. По умолчанию `URL for the link:`.
- **renderingConfig**: Настройте параметры для парсинга Markdown во время предварительного просмотра (не редактируя).
  - **codeSyntaxHighlighting**: Если стоит значение `true`, будет выделено с помощью [highlight.js](https://github.com/isagalaev/highlight.js). По умолчанию `false`. Чтобы использовать эту функцию, вы должны включить highlight.js на вашей странице или передать с помощью опции `hljs`. Например, включить скрипт и CSS-файлы, такие как:<br>`<script src="https://cdn.jsdelivr.net/highlight.js/latest/highlight.min.js"></script>`<br>`<link rel="stylesheet" href="https://cdn.jsdelivr.net/highlight.js/latest/styles/github.min.css">`
  - **hljs**: Инъецируемый экземпляр [highlight.js](https://github.com/isagalaev/highlight.js). Если вы не хотите полагаться на глобальное пространство имен (`window.hljs`), то можно предоставить экземпляр здесь. По умолчанию `undefined`.
  - **markedOptions**: Установить встроенные в обработчик Markdown [опции](https://github.com/chjj/marked#options-1). Остальные `renderingConfig` опции будут иметь приоритет.
  - **singleLineBreaks**: Если стоит значение `false`, отключить парсинг разрывов строк GFM. По умолчанию `true`.
- **shortcuts**: Сочетания клавиш, связанные с этим экземпляром. По умолчанию используется [массив ярлыков](#Горячие-клавиши).
- **showIcons**: Массив для отображения имен иконок. Может использоваться для отображения определенных иконок, скрытых по умолчанию, без полной настройки панели инструментов.
- **spellChecker**: Если стоит значение `false`, то отключить проверку орфографии. По умолчанию `true`.
- **status**: Если стоит значение `false`, то скрыть строку состояния. По умолчанию используется массив встроенных элементов строки состояния.
  - При желании вы можете установить массив элементов строки состояния для добавления в любом порядке. Вы даже можете определить свои собственные элементы строки состояния.
- **styleSelectedText**: Если стоит значение `false`, то убрать класс `CodeMirror-selectedtext`. По умолчанию `true`.
- **syncSideBySidePreviewScroll**: Если стоит значение `false`, отключить синхронизацию прокрутки в режиме бок о бок. По умолчанию `true`.
- **tabSize**: Если установлено, то можно настроить размер табуляции. По умолчанию значение `2`.
- **theme**: Переопределить тему. По умолчанию значение `easymde`.
- **toolbar**: Если стоит значение `false`, то скрыть панель инструментов. По умолчанию используется [массив иконок](#Значки-панели-инструментов).
- **toolbarTips**: Если стоит значение `false`, отключить подсказки кнопок панели инструментов. По умолчанию `true`.

```JavaScript
// Большинство параметров демонстрируют поведение не по умолчанию
export default {
  data () {
    return {
      configs: {
        autofocus: true,
        autosave: {
          enabled: true,
          uniqueId: 'MyUniqueID',
          delay: 1000
        },
        blockStyles: {
          bold: '__',
          italic: '_'
        },
        element: document.getElementById('MyID'),
        forceSync: true,
        hideIcons: ['guide', 'heading'],
        indentWithTabs: false,
        initialValue: 'Hello world!',
        insertTexts: {
          horizontalRule: ['', '\n\n-----\n\n'],
          image: ['![](http://', ')'],
          link: ['[', '](http://)'],
          table: ['', '\n\n| Column 1 | Column 2 | Column 3 |\n| -------- | -------- | -------- |\n| Text     | Text      | Text     |\n\n']
        },
        lineWrapping: false,
        parsingConfig: {
          allowAtxHeaderWithoutSpace: true,
          strikethrough: false,
          underscoresBreakWords: true
        },
        placeholder: 'Type here...',
        previewRender: function(plainText) {
          return customMarkdownParser(plainText) // Возвращает HTML из пользовательского парсера
        },
        previewRender: function(plainText, preview) { // Асинхронный метод
          setTimeout(function(){
            preview.innerHTML = customMarkdownParser(plainText)
          }, 250)

          return 'Loading...'
        },
        promptURLs: true,
        renderingConfig: {
          singleLineBreaks: false,
          codeSyntaxHighlighting: true
        },
        shortcuts: {
          drawTable: 'Cmd-Alt-T'
        },
        showIcons: ['code', 'table'],
        spellChecker: false,
        status: false,
        status: ['autosave', 'lines', 'words', 'cursor'], // Опциональное использование
        status: ['autosave', 'lines', 'words', 'cursor', {
          className: 'keystrokes',
          defaultValue: function(el) {
            this.keystrokes = 0
            el.innerHTML = '0 Keystrokes'
          },
          onUpdate: function(el) {
            el.innerHTML = ++this.keystrokes + ' Keystrokes'
          }
        }], // Другое опциональное использование, с пользовательским элементом строки состояния, который считает нажатия клавиш
        styleSelectedText: false,
        tabSize: 4,
        toolbar: false,
        toolbarTips: false
      }
    }
  }
}
```

#### Значки панели инструментов

Ниже приведены значки встроенной панели инструментов (только некоторые из них включены по умолчанию), которые могут быть реорганизованы по желанию. "Название" является названием иконки, определенным в JS. "Действие" - это либо функция, либо URL для открытия. "Класс" - это класс иконки. "Подсказка" - это маленькая подсказка, появляющаяся с помощью атрибута `title=""`.
Обратите внимание, что подсказки добавляются автоматически и отражают указанное действие, если ему назначена привязка клавиш (т.е. со значением `action`, установленным в `bold`, и `tooltip`, установленным в `Bold`, итоговый текст, который увидит пользователь, будет "Bold (Ctrl-B)").

Кроме того, вы можете добавить разделитель между любыми значками, добавив `"|"` в массив панели инструментов.

Название | Действие | Подсказка<br>Класс
:--- | :----- | :--------------
bold | toggleBold | Bold<br>fa fa-bold
italic | toggleItalic | Italic<br>fa fa-italic
strikethrough | toggleStrikethrough | Strikethrough<br>fa fa-strikethrough
heading | toggleHeadingSmaller | Heading<br>fa fa-header
heading-smaller | toggleHeadingSmaller | Smaller Heading<br>fa fa-header
heading-bigger | toggleHeadingBigger | Bigger Heading<br>fa fa-lg fa-header
heading-1 | toggleHeading1 | Big Heading<br>fa fa-header header-1
heading-2 | toggleHeading2 | Medium Heading<br>fa fa-header header-2
heading-3 | toggleHeading3 | Small Heading<br>fa fa-header header-3
code | toggleCodeBlock | Code<br>fa fa-code
quote | toggleBlockquote | Quote<br>fa fa-quote-left
unordered-list | toggleUnorderedList | Generic List<br>fa fa-list-ul
ordered-list | toggleOrderedList | Numbered List<br>fa fa-list-ol
clean-block | cleanBlock | Clean block<br>fa fa-eraser
link | drawLink | Create Link<br>fa fa-link
image | drawImage | Insert Image<br>fa fa-picture-o
table | drawTable | Insert Table<br>fa fa-table
horizontal-rule | drawHorizontalRule | Insert Horizontal Line<br>fa fa-minus
preview | togglePreview | Toggle Preview<br>fa fa-eye no-disable
side-by-side | toggleSideBySide | Toggle Side by Side<br>fa fa-columns no-disable no-mobile
fullscreen | toggleFullScreen | Toggle Fullscreen<br>fa fa-arrows-alt no-disable no-mobile
guide | [This link](https://markdownguide.org/basic-syntax/) | Markdown Guide<br>fa fa-question-circle

Настройте панель инструментов с помощью опции `toolbar`, например:

```JavaScript
// Настройте только порядок существующих кнопок
export default {
  data () {
    return {
      configs: {
        toolbar: ['bold', 'italic', 'heading', '|', 'quote']
      }
    }
  }
}

// Настройте всю информацию и / или добавьте свои собственные значки
export default {
  data () {
    return {
      configs: {
        toolbar: [{
            name: 'bold',
            action: EasyMDE.toggleBold,
            className: 'fa fa-bold',
            title: 'Bold'
          },
          {
            name: 'custom',
            action: function customFunction(editor){
              // Добавьте свой собственный код
            },
            className: 'fa fa-star',
            title: 'Custom Button'
          },
          '|' // Разделитель
          ...
        ]
      }
    }
  }
}
```

#### Горячие клавиши

EasyMDE предоставляется с рядом горячих клавиш по умолчанию, но они могут быть изменены с помощью параметра конфигурации. Список по умолчанию выглядит следующим образом:

Клавиши (Windows / Linux) | Клавиши (macOS) | Действие
:--- | :--- | :---
*Ctrl-'* | *Cmd-'* | "toggleBlockquote"
*Ctrl-B* | *Cmd-B* | "toggleBold"
*Ctrl-E* | *Cmd-E* | "cleanBlock"
*Ctrl-H* | *Cmd-H* | "toggleHeadingSmaller"
*Ctrl-I* | *Cmd-I* | "toggleItalic"
*Ctrl-K* | *Cmd-K* | "drawLink"
*Ctrl-L* | *Cmd-L* | "toggleUnorderedList"
*Ctrl-P* | *Cmd-P* | "togglePreview"
*Ctrl-Alt-C* | *Cmd-Alt-C* | "toggleCodeBlock"
*Ctrl-Alt-I* | *Cmd-Alt-I* | "drawImage"
*Ctrl-Alt-L* | *Cmd-Alt-L* | "toggleOrderedList"
*Shift-Ctrl-H* | *Shift-Cmd-H* | "toggleHeadingBigger"
*F9* | *F9* | "toggleSideBySide"
*F11* | *F11* | "toggleFullScreen"

Пример, как можно изменить некоторые из сочетаний горячих клавиш:

```JavaScript
export default {
  data () {
    return {
      configs: {
        shortcuts: {
          'toggleOrderedList': 'Ctrl-Alt-K', // изменить toggleOrderedList
          'toggleCodeBlock': null, // отвязать Ctrl-Alt-C
          'drawTable': 'Cmd-Alt-T' // привязать Cmd-Alt-T к действию drawTable, которое не поставляется с ярлыком по умолчанию
        }
      }
    }
  }
}
```

Ярлыки автоматически конвертируются между платформами. Если вы определите ярлык как "Cmd-B", на ПК этот ярлык будет изменен на "Ctrl-B". И наоборот, ярлык, определенный как "Ctrl-B" станет "Cmd-B" для пользователей Mac.

Список действий, которые могут быть связаны, совпадает со списком встроенных действий, доступных для [кнопок панели инструментов](#Значки-панели-инструментов).

## Обработка событий
Вы можете найти список событий здесь: https://codemirror.net/doc/manual.html#events

```JavaScript
var easymde = new EasyMDE();
easymde.codemirror.on("change", function(){
	console.log(easymde.value());
});
```

## Удаление EasyMDE из текстовой области
Вы можете вернуться к исходной текстовой области, вызвав метод `toTextArea`. Обратите внимание, что это очищает автосохранение (если было включено), связанное с ним. Текстовое поле сохранит любой текст из уничтоженного экземпляра EasyMDE.

```JavaScript
var easymde = new EasyMDE();
...
easymde.toTextArea();
easymde = null;
```

## Полезные методы
Следующие очевидные методы могут быть полезны при разработке с EasyMDE.

```js
var easymde = new EasyMDE();
easymde.isPreviewActive(); // returns boolean
easymde.isSideBySideActive(); // returns boolean
easymde.isFullscreenActive(); // returns boolean
easymde.clearAutosavedValue(); // no returned value
```
