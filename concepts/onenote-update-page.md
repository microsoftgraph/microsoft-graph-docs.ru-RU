---
title: Обновление содержимого страниц OneNote
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 06594d0c5f584330b16d523e4f7dc2e8de4be080
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103979"
---
# <a name="update-onenote-page-content"></a>Обновление содержимого страниц OneNote

**Область применения**: пользовательские записные книжки в OneDrive | корпоративные записные книжки в Microsoft 365


Чтобы обновить содержимое страницы OneNote, необходимо отправить запрос PATCH в конечную точку *content* страницы:

`PATCH ../notes/pages/{id}/content`</p>

Отправьте объект изменений JSON в тексте сообщения. Если запрос будет выполнен успешно, Microsoft Graph вернет код состояния HTTP 204.


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Создание URI запроса

Чтобы создать URI запроса, начните с корневого URL-адреса службы:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Затем добавьте конечную точку *content* страницы:

- **Получение HTML-кода страницы и всех определенных значений *data-id***<br/><br/>`../pages/{id}/content`   

- **Получение HTML-кода страницы, всех определенных значений *data-id* и всех созданных значений *id***<br/><br/>`../pages/{page-id}/content?includeIDs=true` 

Значения **data-id** и **id** используются в качестве идентификаторов **target** для элементов, которые требуется изменить.

 
Полный URI запроса будет выглядеть так:<br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


Узнайте больше о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Составление текста сообщения

HTML-код страницы OneNote содержит текст, изображения и другое содержимое, структурированные с помощью таких элементов, как **div**, **img** и **ol**. Для обновления содержимого страницы OneNote необходимо добавлять и заменять элементы HTML на странице.

Изменения отправляются в тексте сообщения в виде массива объектов JSON. В каждом объекте указываются целевой элемент, новое содержимое HTML и действия, которые нужно выполнить с содержимым.

Следующий массив определяет два изменения. Первое вставляет изображение над абзацем в качестве элемента того же уровня, а второе добавляет элемент в список в качестве последнего дочернего элемента.

> [!NOTE]
> При обновлении изображения на OneNote странице вы не можете использовать ссылки www. Служба не будет пытаться скачивать случайные ресурсы. Вместо этого изображение должно быть частью запроса либо url-адресом изображений, либо имям части многопартийного запроса.

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

См. [другие примеры](#example-requests).


### <a name="attributes-for-json-change-objects"></a>Атрибуты объектов JSON

Для определения объектов JSON в запросах PATCH используются атрибуты **target**, **action**, **position** и **content**.

#### <a name="target"></a>target

Обновляемый элемент. Значением должен быть один из следующих идентификаторов:

| Идентификатор | Описание |  
|------|------|  
| #{data-id} | <p>Этот идентификатор при желании определяется для элементов входного HTML-кода при [создании](onenote-create-page.md) или [обновлении страницы](onenote-update-page.md). Добавьте перед этим значением префикс #.</p><p> Пример:<br/>`'target':'#intro'` задает в качестве целевого элемент `<div data-id="intro" ...>`</p> |  
| id | <p>Это [сгенерированный идентификатор](#generated-ids) из Microsoft Graph, необходимый для большинства операций замены. Не добавляйте перед ним префикс #.</p><p> Пример:<br/>`'target':'div:{33f8a2...}{37}'` задает в качестве целевого элемент `<div id="div:{33f8a2...}{37}" ...>`</p><p>Не путайте эти идентификаторы со значениями **id**, определенными во [входном HTML-коде](onenote-input-output-html.md). Все значения **id**, отправляемые во входном HTML-коде, отклоняются.</p> |  
| body | Ключевое слово, указывающее на первый разделитель на странице. Не добавляйте перед ним префикс #. |  
| title | Ключевое слово, указывающее на заголовок страницы. Не добавляйте перед ним префикс #. |  
 
#### <a name="action"></a>action

Действие, которое нужно выполнить с целевым элементом. См. [поддерживаемые действия для элементов](#supported-elements-and-actions).

| Действие | Описание |  
|------|------|  
| append | <p>Добавляет указанное содержимое к целевому элементу в качестве первого или последнего дочернего элемента, в зависимости от значения атрибута **position**.</p><p>Применяется только к элементам **body**, **div**, **ol** и **ul**.</p> |  
| insert | Добавляет указанное содержимое в качестве элемента того же уровня перед целевым элементом или после него, в зависимости от значения атрибута **position**. |  
| prepend | <p>Добавляет указанное содержимое к целевому элементу в качестве первого дочернего элемента. Сокращение от действия **append** + **before**.</p><p>Применяется только к элементам **body**, **div**, **ol** и **ul**.</p> |  
| replace | <p>Заменяет целевой элемент указанным содержимым.</p><p>Для большинства действий **replace** необходимо использовать [сгенерированный идентификатор](#generated-ids) целевого элемента (кроме элементов **img** и **object** внутри разделителя, которые также поддерживают использование **data-id**).</p> |  
 
#### <a name="position"></a>position

Место для добавления предоставленного контента относительно целевого элемента. Если атрибут опущен, по умолчанию он принимает значение **after**.

| Position | Описание |  
|------|------|  
| after (по умолчанию) |<p>С действием **append**: последний дочерний элемент целевого элемента.</p><p>С действием **insert**: следующий элемент того же уровня, что и целевой элемент.</p> |
| before | <p>С действием **append**: первый дочерний элемент целевого элемента.</p><p>С действием **insert**: предыдущий элемент того же уровня, что и целевой элемент.</p> |

#### <a name="content"></a>content

Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если в содержимом есть двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands (см. [пример](#multipart-request-with-binary-content)). 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a>Сгенерированные идентификаторы
Microsoft Graph создает значения **id** для тех элементов на странице, которые можно обновить. Чтобы получить сгенерированные идентификаторы, используйте выражение строки `includeIDs=true` в запросе GET:

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> **Примечание.** API отклоняет все значения **id**, определенные во [входном HTML-коде](onenote-input-output-html.md) запросов create-page и update-page.

Ниже показаны сгенерированные идентификаторы для абзаца и изображения в [выходном HTML-коде](onenote-input-output-html.md) страницы.

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

Сгенерированные значения **id** могут изменяться после обновления страницы, поэтому вам следует получить текущие значения до создания использующего их PATCH-запроса.
 
Вы можете указать целевые элементы, используя значение **data-id** или **id**, как указано ниже.

- Для действий **append** и **insert** в качестве целевого значения можно использовать любой идентификатор.
- Для действий **replace** необходимо использовать сгенерированный идентификатор для всех элементов, кроме заголовка, а также изображений и объектов, находящихся внутри разделителя. 
  - Чтобы заменить заголовок, используйте ключевое слово **title**. 
  - Чтобы заменить изображения и объекты, находящиеся внутри разделителя, используйте атрибут **data-id** или **id**.

В приведенном ниже примере используется значение **id** целевого элемента. Не используйте префикс # со сгенерированным идентификатором.

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a>Поддерживаемые элементы и действия

Многие элементы на странице можно обновлять, но каждый тип элемента поддерживает определенные действия. Ниже показаны поддерживаемые целевые элементы и поддерживаемые ими действия по обновлению.

| Элемент | Заменить | Добавление дочернего элемента | Вставка элемента того же уровня |  
|------|:------:|:------:|:------:|  
| body<br /> (делает целевым первый разделитель на странице) | нет | **да** | нет |  
| div<br /> ([абсолютное расположение](onenote-abs-pos.md)) | нет | **да** | нет |  
| div<br /> (внутри разделителя) | **да**<br/>(только идентификатор) | **да** | **да** |   
| img, object<br /> (внутри разделителя) | **да** | нет | **да** |   
| ol, ul | **да**<br/>(только идентификатор) | **да** | **да** |   
| table | **да**<br/>(только идентификатор) | нет | **да** |   
| p, li, h1-h6 | **да**<br/>(только идентификатор) | нет | **да** |   
| title | **да** | нет | нет |  
 
<br/>

Указанные ниже элементы не поддерживают никаких действий обновления.

- img ([абсолютное расположение](onenote-abs-pos.md))
- object ([абсолютное расположение](onenote-abs-pos.md))
- tr, td
- meta
- head
- span
- a
- Теги style


<a name="examples"></a>

## <a name="example-requests"></a>Примеры запросов

Запрос на обновление содержит одно или несколько изменений, представленных в виде объектов JSON. Эти объекты могут определять различные целевые элементы на странице, а также различные действия и содержимое для целевых элементов.

Следующие примеры включают объекты JSON, используемые в запросах PATCH, а также готовые запросы PATCH:

- [Добавление дочерних элементов](#append-child-elements)
- [Вставка элементов того же уровня](#insert-sibling-elements)
- [Замена элементов](#replace-elements)
- [Выполнение запросов PATCH](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a>Добавление дочерних элементов

Действие **append** добавляет дочерний элемент в элемент **body**, **div** (в составе разделителя), **ol** или **ul**. Атрибут **position** определяет, следует ли добавить дочерний элемент перед целевым элементом или после него. Расположение по умолчанию — **after**.

#### <a name="append-to-a-div"></a>Добавление в разделитель

В приведенном ниже примере в элемент **div1** добавляется два дочерних узла. Изображение добавляется в качестве первого дочернего элемента, а абзац — в качестве последнего. 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a>Добавление к элементу *body*

Вы можете использовать сокращение **body** для добавления дочернего элемента внутри первого разделителя на любой странице.

В приведенном ниже примере в первый разделитель на странице добавляется два абзаца: один в качестве первого дочернего элемента, а другой — в качестве последнего. Не используйте префикс # с целевым элементом **body**. В этом примере действие **prepend** используется в качестве сокращения от действия **append** + **before**.

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a>Добавление в список

В следующем примере элемент списка добавляется в качестве последнего дочернего элемента к целевому списку. Свойство **list-style-type** определено, так как элемент использует стиль списка не по умолчанию.

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a>Вставка элементов того же уровня

Действие **insert** добавляет элемент того же уровня в целевой элемент. Атрибут **position** определяет, где следует вставлять элемент: до или после целевого элемента. По умолчанию задано положение **after**. См. [элементы, поддерживающие действие **insert**](#supported-elements-and-actions).

#### <a name="insert-siblings"></a>Вставка элементов того же уровня

В следующем примере два узла того же уровня добавляются на страницу. Над элементом **para1** добавляется изображение, а под элементом **para2** — абзац.

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a>Замена элементов

Вы можете использовать **data-id** или сгенерированный **id** в качестве целевого значения для замены элементов **img** и **object** внутри разделителя. Чтобы заменить заголовок, используйте ключевое слово **title**. Для всех остальных [элементов, поддерживающих действие **replace**](#supported-elements-and-actions), необходимо использовать сгенерированный идентификатор.

#### <a name="replace-an-image"></a>Замена изображения

В приведенном ниже примере изображение заменяется разделителем; в качестве целевого элемента используется **data-id** изображения. 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a>Обновление таблицы 

Этот пример демонстрирует, как обновить таблицу при помощи ее сгенерированного ИД. Замена элементов **tr** и **td** не поддерживается, но вы можете заменить таблицу целиком.

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a>Изменение заголовка 

В этом примере показано, как изменить заголовок страницы. Чтобы изменить заголовок, используйте ключевое слово **title** в качестве целевого значения. Не используйте префикс # в целевом заголовке.

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a>Обновление элемента списка дел

В приведенном ниже примере используется действие replace, чтобы перевести флажок в списке дел в состояние "Выполнено".

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

Дополнительные сведения об использовании атрибута [data-tag](onenote-note-tags.md) см. в **этой статье**.


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a>Примеры выполнения запросов PATCH

В следующих примерах показаны готовые запросы PATCH.

#### <a name="request-with-text-content-only"></a>Запрос с текстовым содержимым

В приведенном ниже примере показан запрос PATCH, в котором используется тип контента **application/json**. Этот формат можно использовать, если контент не содержит двоичных данных.

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a>Составной запрос с двоичным содержимым 

В приведенном ниже примере показан составной запрос PATCH, включающий двоичные данные. Составные запросы включают часть Commands, в которой указывается тип контента **application/json** и предоставляется массив объектов изменений JSON. Другие части данных могут содержать двоичные данные. Как правило, имена частей представляют собой строки, к которым добавлено текущее время в миллисекундах или случайный GUID.

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a>Информация о запросах PATCH и соответствующих ответах

| Данные запроса | Описание |  
|------|------|  
| Протокол | Все запросы используют протокол SSL/TLS для HTTPS. |  
| Заголовок Authorization | <p>`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</p><p>Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401. См. статью [Проверка подлинности и разрешения](permissions-reference.md).</p> |  
| Заголовок Content-Type | <p>`application/json` для массива объектов изменений JSON, отправленного либо непосредственно в тексте сообщения, либо в обязательной части Commands [составных запросов](#multipart-request-with-binary-content).</p><p>Составные запросы необходимы при отправке двоичных данных и используют тип контента `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` — это строка, обозначающая начало и конец каждой части данных.</p> |  

<br/> 

| Данные в отклике | Описание |  
|------|------|  
| Код успешного завершения | Код состояния HTTP 204. Данные JSON не возвращаются по PATCH-запросу. |  
| Ошибки | Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md). |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Составление корневого URL-адреса службы Microsoft Graph

Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote:

`https://graph.microsoft.com/{version}/me/onenote/`

Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph. Значение `v1.0` предназначено для стабильного производственного кода. Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.

Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым). Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Использование [API Graph для Azure AD](/previous-versions/azure/ad/graph/api/api-catalog)


> **Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.



<a name="permissions"></a>

## <a name="permissions"></a>Разрешения

Для обновления страниц OneNote необходимо запрашивать соответствующие разрешения. Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.

- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md).
   

<a name="see-also"></a>

## <a name="see-also"></a>См. также

- [Добавление изображений и файлов](onenote-images-files.md)
- [Интеграция с OneNote](integrate-with-onenote.md)
- [Блог разработчиков OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»](/answers/topics/microsoft-graph-notes.html)
- [Репозитории GitHub OneNote](https://go.microsoft.com/fwlink/?LinkID=390178)
