---
title: Создание абсолютно позиционированных элементов на страницах OneNote с помощью API OneNote
description: Используйте атрибуты с поддержкой абсолютных данных и стиля для создания абсолютных позиционированных элементов на странице, включая несколько прямых элементов div, img и дочерних элементов объекта.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 9cc2ecb5a80630ce5d2d763fd01467a68a1d8828
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446206"
---
# <a name="create-absolute-positioned-elements-on-onenote-pages"></a>Создание элементов с абсолютным положением на страницах OneNote

В тексте страницы OneNote может содержаться много прямых (`div`, `img`) и дочерних (`object`) элементов, которые можно разместить независимо друг от друга на странице.

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a>Атрибуты и поведение при расположении

Чтобы создать элементы с абсолютным положением на странице, используйте атрибуты `data-absolute-enabled` и [`style`](#supported-css-style-attributes), как показано ниже.

- Элемент body должен указывать `data-absolute-enabled="true"`. Если он опущен или имеет значение `false`, весь контент в элементе body отображается в элементе `_default` с абсолютным положением, созданным API, и все параметры положения будут проигнорированы.

- Только элементы `div`, `img` и `object` могут иметь абсолютное положение. 

- Для элементов с абсолютным положением должен быть задан параметр `style="position:absolute"`.

- Элементы с абсолютным положением должны быть прямыми дочерними элементами элемента `body`. Любой прямой дочерний элемент элемента body, не являющийся элементом `div`, `img` или `object` с абсолютным положением, отображается в виде статичного контента внутри элемента div `_default` с абсолютным положением.

- Элементы с абсолютным положением размещаются согласно указанным для них координатам левого верхнего угла относительно начального положения 0:0, соответствующего левому верхнему углу страницы над областью заголовка.

- Если у элемента с абсолютным положением опущена верхняя или левая координата, для этой координаты применяется соответствующее значение, используемое по умолчанию: `top:120px` или `left:48px`. Эти координаты, используемые по умолчанию, указывают положение непосредственно под областью заголовка. Помните, что если не указывать координаты элементов, последние будут накладываться друг на друга.

- Элементы с абсолютным положением не должны быть вложенными и не должны содержать элементы с заданными положениями. API игнорирует все параметры положения, указанные во вложенных элементах внутри элемента div с абсолютным положением, отображает вложенный контент внутри родительского элемента div с абсолютным положением и возвращает предупреждение через свойство **api.diagnostics** в ответе.


### <a name="example"></a>Пример

В примере ниже показан прямой дочерний элемент `p`, элемент div с абсолютным положением и элемент div с неабсолютным положением.

#### <a name="input-html"></a>Входной HTML-код  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

API отрисовывает элемент div с неабсолютным положением в элементе div, используемом по умолчанию. Обратите внимание, что система игнорирует вложенные теги `<div>`, так как в них не определено никакой семантической информации (например, `data-id`).

#### <a name="output-html"></a>Выходной HTML-код 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a>Пример

В примере ниже показано, как создать страницу, которая содержит один элемент div с абсолютным положением и одно изображение с абсолютным положением.


#### <a name="input-html"></a>Входной HTML-код  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
API OneNote оценивает входной HTML-код и сохраняет весь семантический контент и информацию о структуре, которые поддерживает OneNote. Полученная в результате страница отображается, как показано на рисунке ниже (но без видимых границ для элемента div и изображения). 

![Полученная в результате страница с элементом div и изображением с абсолютными положениями](images/abs-pos.png)

Обратите внимание на изменение незначимого вложенного элемента div по сравнению со входным HTML-кодом. API сохраняет контент, содержащийся в элементе div, но игнорирует теги `<div>`, так как в элементе div не определена семантическая информация (например, `data-id`).

Дополнительные сведения о том, как API OneNote обрабатывает входной и выходной HTML-код, см. в статье [Входной и выходной HTML-код на страницах OneNote](onenote-input-output-html.md).

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a>Поддерживаемые атрибуты стиля CSS

Для всех элементов с абсолютными положениями можно указать положения левого верхнего угла. Для элемента div и изображения можно указать ширину. Кроме того, для изображений можно указать высоту. Пример:

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| Атрибут | Поддерживаемый элемент | Описание |  
|:------|:------|:------|  
| top | div, img, object | Координата верхней границы элемента по оси Y; только в пикселях. По умолчанию используется значение 120 пикселей.<br/><br/>Пример: `top:140px` |  
| left |  div, img, object  | Координата левой границы элемента по оси X; только в пикселях. По умолчанию используется значение 48 пикселей.<br/><br/>Пример: `left:95px` |  
| width |  div, img  | Ширина элемента; только в пикселях.<br/><br/>Пример: `width:480px` |  
| height | img | Высота элемента; только в пикселях. Для элементов div высота рассчитывается в среде выполнения, и система игнорирует любое заданное значение высоты.<br/><br/>Пример: `height:665px` |  
 
Система игнорирует другие атрибуты положения, например `z-index`. Для изображений с абсолютными положениями можно использовать атрибут `data-render-src` или `src`.


<a name="request-response-info"></a>

## <a name="response-information"></a>Информация в ответе

API OneNote возвращает указанные ниже сведения в ответе.

| Данные в отклике | Описание |  
|:------|:------|  
| Код успешного завершения действия | Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH. |  
| Ошибки | Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md). |  
  


<a name="permissions"></a>

## <a name="permissions"></a>Разрешения

Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения. Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.

#### <a name="permissions-for-post-pages"></a>Разрешения для запросов POST со страницами 

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  


#### <a name="permissions-for-patch-pages"></a>Разрешения в случае запросов PATCH для страниц 

- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md#notes-permissions).


<a name="see-also"></a>

## <a name="see-also"></a>См. также

- [Создание страниц OneNote](onenote-create-page.md)
- [Обновление содержимого страницы OneNote](onenote-update-page.md)
- [Интеграция с OneNote](integrate-with-onenote.md)
- [Блог разработчиков OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»](/answers/topics/microsoft-graph-notes.html)
- [Репозитории GitHub OneNote](https://go.microsoft.com/fwlink/?LinkID=390178)
