---
title: Получение содержимого и структуры OneNote с помощью Microsoft Graph
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: f3e40662d2e750514ef6c71b3faa604e13ccc773
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921660"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a>Получение содержимого и структуры OneNote с помощью Microsoft Graph

**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.

Чтобы получить содержимое и структуру OneNote, необходимо отправить запрос GET к целевой конечной точке. Пример:

`GET ../onenote/pages/{id}`

Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 200 и запрашиваемые объекты или содержимое. Объекты OneNote возвращаются в виде объектов JSON, соответствующих спецификации OData версии 4.0.

С помощью параметров строки запроса вы можете фильтровать запросы и повышать производительность.


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Создание URI запроса

Чтобы создать URI запроса, начните с корневого URL-адреса службы:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Затем добавьте конечную точку нужного ресурса. ([Пути к ресурсам](#resource-paths-for-get-requests) показаны в следующем разделе.)

Полный URI запроса будет выглядеть так, как в одном из следующих примеров:

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> **Примечание.** Узнайте больше о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a>Пути к ресурсам для запросов GET

Используйте приведенные ниже пути к ресурсам, чтобы получать страницы, разделы, группы разделов, записные книжки, а также изображения или файлы.

- [Коллекция Page](#page-collection)
- [Объект Page](#page-entity)
- [Предварительный просмотр страницы](#page-preview)
- [HTML-контент страницы](#page-html-content)
- [Коллекция Section](#section-collection)
- [Объект Section](#section-entity)
- [Коллекция SectionGroup](#sectiongroup-collection)
- [Объект SectionGroup](#sectiongroup-entity)
- [Коллекция Notebook](#notebook-collection)
- [Объект Notebook](#notebook-entity)
- [Ресурс изображений или других файлов](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a>Коллекция Page

Получение страниц (метаданных) из всех записных книжек.

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

Получение страниц (метаданных) из определенного раздела.

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
Параметр строки запроса `search` доступен только для пользовательских записных книжек.

По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.

Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.

По умолчанию в ответ на запросы *GET для страниц* возвращаются только первые 20 записей. В ответах на запросы, в которых не указан параметр **top**, возвращается ссылка `@odata.nextLink`, с помощью которой можно получить следующие 20 записей.

Для коллекции страниц в разделе используйте параметр **pagelevel**, чтобы возвращать уровень отступа страниц и их порядок в разделе. 

#### <a name="example"></a>Пример

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a>Объект Page

Получение метаданных определенной страницы. 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

Запросы страниц могут разворачивать свойства **parentNotebook** и **parentSection**.

Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.

С помощью параметра **pagelevel** можно вернуть уровень отступа страницы и ее порядковый номер в родительском разделе. 

#### <a name="example"></a>Пример

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a>Предварительный просмотр страницы

Получение текста и изображений на странице для предварительного просмотра.

`../pages/{page-id}/preview`

<br/>


Отклик JSON содержит часть контента для предварительного просмотра, благодаря которому пользователи могут узнать, что находится на странице.

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

Свойство **previewText** содержит фрагмент текста со страницы. Microsoft Graph возвращает полные фразы длиной до 300 символов. 

Если на странице есть изображение, подходящее для предварительного просмотра, то свойство **href** объекта **previewImageUrl** будет содержать ссылку на общедоступный [ресурс изображения](#image-or-other-file-resource). Эту ссылку можно использовать в коде HTML. Если не сделать этого, свойство **href** возвратит значение NULL.

#### <a name="example"></a>Пример 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a>HTML-контент страницы

Получение HTML-контента страницы.

`../pages/{page-id}/content[?includeIDs]`

(*Дополнительные сведения о [возвращаемом HTML-контенте](onenote-input-output-html.md)*.) 

<br/>

Указав в строке запроса параметр **includeIDs=true**, можно получить созданные идентификаторы, используемые для [обновления страницы](onenote-update-page.md).



<a name="get-sections"></a>

### <a name="section-collection"></a>Коллекция Section

Получение всех разделов всех записных книжек, принадлежащих пользователю, включая разделы из вложенных групп разделов.

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Получение всех разделов, вложенных непосредственно в определенную группу разделов.

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Получение всех разделов, вложенных непосредственно в определенную записную книжку.

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.

По умолчанию для разделов используется порядок сортировки `name asc`.

Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.



<a name="get-section"></a>

### <a name="section-entity"></a>Объект Section

Получение определенного раздела.

`../sections/{section-id}[?select,expand]` 

<br/>

Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.

Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a>Коллекция SectionGroup

Получение всех групп разделов из всех записных книжек, принадлежащих пользователю, включая вложенные.

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Получение всех групп разделов, вложенных непосредственно в определенную записную книжку. 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.

По умолчанию для групп разделов используется порядок сортировки `name asc`.

Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a>Объект SectionGroup

Получение определенной группы разделов.

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.

Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a>Коллекция Notebook

Получение всех записных книжек, принадлежащих пользователю. 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.

По умолчанию для записных книжек используется порядок сортировки `name asc`. 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a>Объект Notebook

Получение определенной записной книжки.

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a>Ресурс изображений или других файлов

Получение двоичных данных определенного ресурса. 

`../resources/{resource-id}/$value` 

<br/>

URI ресурса файла можно найти в [выходном HTML-коде](onenote-input-output-html.md) страницы.

Например, тег **img** содержит конечные точки для исходного изображения в атрибуте **data-fullres-src** и оптимизированное изображение в атрибуте **src**. 

#### <a name="example"></a>Пример

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

Тег **object** содержит конечную точку файлового ресурса в атрибуте **data**. 

#### <a name="example"></a>Пример

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> **Примечание.** Получение коллекции ресурсов не поддерживается. 

При получении файлового ресурса не требуется включать в запрос тип контента **Accept**.

Дополнительные сведения о запросах GET см. в следующих статьях документации по API REST Microsoft Graph:

- [Запрос GET для страниц](/graph/api/page-get?view=graph-rest-1.0)
- [GET Sections](/graph/api/section-get?view=graph-rest-1.0)
- [GET SectionGroups](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [Запрос GET для записных книжек](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a>Примеры запросов GET

Вы можете запрашивать объекты OneNote и содержимое страницы поиска, чтобы получать только нужные вам сведения. Ниже показаны некоторые способы использования [поддерживаемых параметров строки](#supported-odata-query-string-options) в запросах GET к Microsoft Graph. 

**Помните:**

- Все запросы GET начинаются с [корневого URL-адреса службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url). <br/><br/>**Примеры**: `https://www.onenote.com/api/v1.0/me/notes` и `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`.

- Пробелы в строке запроса URL следует кодировать как %20.<br/><br/>**Пример**: `filter=title%20eq%20'biology'`.

- В случае имен свойств и сравнения строк OData учитывается регистр. Рекомендуем использовать функцию OData **tolower** для сравнения строк.<br/><br/>**Пример**: `filter=tolower(name) eq 'spring'`.
 

### <a name="search--filter"></a>search и filter  

Получение всех страниц с термином *recipe*, созданных определенным приложением (`search` доступен только для пользовательских записных книжек).

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a>search и select  

Получение заголовка, клиентских ссылок OneNote и ссылки **contentUrl** для всех страниц, содержащих термин *golgi app* (`search` доступен только для пользовательских записных книжек).

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a>expand 

Получение всех записных книжек, а также разворачивание их разделов и групп разделов.  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

Получение определенной группы разделов и разворачивание ее разделов и групп разделов.  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

Получение страницы и разворачивание ее родительского раздела и родительской записной книжки.

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a>expand (несколько уровней)  

Получение всех записных книжек и разворачивание их разделов и групп разделов, а также разворачивание всех разделов в каждой группе разделов.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> **Примечание.** Разворачивание родительских элементов объектов или разворачивание дочерних элементов объектов создает циклическую ссылку и не поддерживается.

 
### <a name="expand--select-multiple-levels"></a>expand и select (несколько уровней)  

Получение имени и ссылки **self** для определенной группы разделов, а также получение имени и ссылок **self** для всех ее разделов.  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

Получение имени и ссылки **self** для всех разделов, а также получение имени и времени создания родительской записной книжки каждого раздела.  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
Получение названий и идентификаторов всех страниц, а также получение названия родительского раздела и родительской записной книжки.

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a>expand и levels (несколько уровней)  

Получение всех записных книжек, разделов и групп разделов.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a>filter

Получение всех разделов, созданных в октябре 2014 г.

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

Получение страниц, созданных определенным приложением с 1 января 2015 г.

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a>filter и expand  

Получение всех страниц определенной записной книжки. По умолчанию API возвращает 20 записей.

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке *School*. При сравнении строк OData учитывается регистр, поэтому рекомендуем использовать функцию **tolower**.

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a>filter, select и orderby   

Получение имени и ссылки **pagesUrl** для всех разделов, имена которых содержат термин *spring*. Упорядочивание разделов по дате последнего изменения.

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a>orderby

Получение первых 20 страниц, отсортированных по свойству **createdByAppId** и времени создания (по убыванию). По умолчанию API возвращает 20 записей.

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a>search, filter и top 

Получение пяти последних страниц, созданных с 1 января 2015 г. и содержащих фразу *cell division*. По умолчанию API возвращает 20 записей. Максимальное количество записей — 100. Порядок сортировки по умолчанию для страниц: `lastModifiedTime desc` (`search` доступен только для пользовательских записных книжек).

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a>search, filter, top и skip  

Получение пяти следующих страниц в результирующем наборе (`search` доступен только для пользовательских записных книжек).

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

Получение еще пяти (`search` доступен только для пользовательских записных книжек).

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> **Примечание.** Если параметры **search** и **filter** применяются к одному запросу, результаты включают только те объекты, которые соответствуют обоим условиям.
 
### <a name="select"></a>select

Получение имени, времени создания и ссылки **self** для всех разделов в записных книжках пользователя.

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

Получение названия, времени создания и клиентских ссылок OneNote для определенной страницы.

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a>select, expand и filter (несколько уровней)  

Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке по умолчанию пользователя.

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a>top, select и orderby 

Получение названия и ссылки **self** для первых 50 страниц, упорядоченных по названию в алфавитном порядке. По умолчанию API возвращает 20 записей. Максимальное количество записей — 100. По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a>skip, top, select и orderby  

Получение страниц с 51 по 100. По умолчанию API возвращает 20 записей, а максимальное количество составляет 100.

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> **Примечание.** Запросы GET для страниц, которые восстанавливают количество записей по умолчанию (то есть в них не указывается выражение **top**), возвращают в ответе ссылку **\@odata.nextLink**, с помощью которой можно получить следующие 20 записей.
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a>Поддерживаемые параметры строки запроса OData

Вы можете настраивать запросы GET к Microsoft Graph, используя параметры строки запроса OData, и получать только нужную информацию. Они также могут повышать производительность, уменьшая количество вызовов службы и размер полезных данных ответа.

> **Примечание.** Для удобства чтения в примерах из этой статьи не используется код %20, которым нужно заменять пробелы в строке запроса URL: `filter=isDefault%20eq%20true`
 
| Параметр запроса | Пример и описание |  
|------|------|  
| count | <p>`count=true`</p><p>Количество объектов в коллекции. Значение возвращается в свойстве **\@odata.count** ответа.</p> |  
| expand | <p>`expand=sections,sectionGroups`</p><p>Свойства навигации, которые следует вернуть в тексте ответа. Для выражений **expand** поддерживаются следующие свойства:<br /> страницы: **parentNotebook**, **parentSection**;<br /> разделы: **parentNotebook**, **parentSectionGroup**;<br /> группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;<br /> записные книжки: **sections**, **sectionGroups**.</p><p>По умолчанию запросы GET для страниц разворачивают **parentSection** и выделяют свойства раздела **id**, **name** и **self**. По умолчанию запросы GET для разделов и групп разделов разворачивают как **parentNotebook**, так и **parentSectionGroup**, а также выделяют родительские свойства **id**, **name** и **self**.</p><p>Может использоваться для одного объекта или коллекции.<br />Свойства следует разделять запятыми.<br />В именах свойств учитывается регистр.</p> |   
| filter | <p>`filter=isDefault eq true`</p><p>Логическое выражение, указывающее, следует ли включать запись в набор результатов. Поддерживаются следующие функции и операторы OData:<br /> — операторы сравнения: **eq**, **ne**, **gt**, **ge**, **lt**, **le**;<br /> — логические операторы: **and**, **or**, **not**;<br /> — строковые функции: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**.</p><p>В случае имен [свойств](#onenote-entity-properties) и сравнения строк OData учитывается регистр. Рекомендуем использовать функцию OData **tolower** для сравнения строк.<br /><br />**Пример**: `filter=tolower(name) eq 'spring'`.</p> |  
| orderby | <p>`orderby=title,createdTime desc`</p><p>
            [Свойства](#onenote-entity-properties) для сортировки с необязательным порядком сортировки **asc** (по умолчанию) или **desc**. Вы можете сортировать по любому свойству сущности в запрошенной коллекции.</p><p>По умолчанию для записных книжек, разделов и групп разделов используется порядок сортировки `name asc`, а для страниц — `lastModifiedTime desc` (сначала отображается последняя измененная страница).</p><p>Разделяйте свойства запятыми и указывайте их в порядке применения. В именах свойств учитывается регистр.</p> |  
| search | <p>`search=cell div`</p><p>Доступен только для пользовательских записных книжек.</p><p>Термин или фраза, которую нужно найти в заголовке и тексте страницы, замещающем тексте изображений и распознанном тексте. По умолчанию поисковые запросы возвращают результаты, отсортированные по релевантности.</p><p>OneNote использует полнотекстовый поиск Bing для поддержки поиска фраз, выделения корней, игнорирования орфографических ошибок, релевантности и ранжирования, разбиения слов, разных языков и других функций полнотекстового поиска. В строках search учитывается регистр.</p><p>Применяется только к страницам записных книжек, принадлежащих пользователю. Индексированное содержимое является личным и доступно только владельцу. Страницы, защищенные паролем, не индексируются. Применяется только к конечной точке `pages`.</p> |  
| select | <p>`select=id,title`</p><p>Возвращаемые [свойства](#onenote-entity-properties). Может использоваться для одного объекта или коллекции. Свойства следует разделять запятыми. В именах свойств учитывается регистр.</p> |  
| skip | <p>`skip=10`</p><p>Количество записей, которое следует пропустить в наборе результатов. Обычно используется для разбиения результатов на страницы.</p> |  
| top | <p>`top=50`</p><p>Количество записей, которое следует вернуть в наборе результатов, до 100. Значение по умолчанию — 20.</p> |  

В Microsoft Graph также доступен параметр строки запроса `pagelevel`, с помощью которого можно получить уровень и порядок страниц в родительском разделе. Применяется только к запросам страниц в определенном разделе и запросам определенной страницы. 

#### <a name="examples"></a>Примеры 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a>Поддерживаемые операторы и функции OData

Microsoft Graph поддерживает указанные ниже функции и операторы OData в выражениях **filter**. Используя выражения OData, помните:

- Пробелы в строке запроса URL необходимо заменять кодом `%20`.<br/><br/>**Пример:** `filter=isDefault%20eq%20true`.

- В случае имен свойств и сравнения строк OData учитывается регистр. Рекомендуем использовать функцию OData **tolower** для сравнения строк.<br/><br/>**Пример:** `filter=tolower(name) eq 'spring'`


| Оператор сравнения | Пример |  
|------|------|  
| eq<br />(равно) | `createdByAppId eq '{app-id}'` |  
| ne<br />(не равно) | `userRole ne 'Owner'` |  
| gt<br />(больше) | `createdTime gt 2014-02-23` |  
| ge<br />(больше или равно) | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| lt<br />(меньше) | `createdTime lt 2014-02-23` |  
| le<br />(меньше или равно) | `lastModifiedTime le 2014-02-23` |  

<br/>

| Логический оператор | Пример |  
|------|------|  
| и | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| Кроме того: | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| 
not | `not contains(tolower(title),'school')` |  

<br/>
  
| Строкова функция | Пример |  
|------|------|   
| contains | `contains(tolower(title),'spring')` |  
| endswith | `endswith(tolower(title),'spring')` |  
| startswith | `startswith(tolower(title),'spring')` |  
| length | `length(title) eq 19` |  
| indexof | `indexof(tolower(title),'spring') eq 1` |  
| substring | `substring(tolower(title),1) eq 'spring'` |  
| tolower | `tolower(title) eq 'spring'` |  
| toupper | `toupper(title) eq 'SPRING'` |  
| trim | `trim(tolower(title)) eq 'spring'` |  
| concat | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a>Свойства объектов OneNote

Выражения запроса **filter**, **select**, **expand** и **orderby** могут включать свойства объектов OneNote. 

#### <a name="example"></a>Пример

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

Для имен свойств в выражениях запроса учитывается регистр.

Список свойств и типы свойств см. в следующих статьях документации по API REST Microsoft Graph:

- [Запрос GET для страниц](/graph/api/page-get?view=graph-rest-1.0)
- [GET Sections](/graph/api/section-get?view=graph-rest-1.0)
- [GET SectionGroups](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [Запрос GET для записных книжек](/graph/api/notebook-get?view=graph-rest-1.0) 



Параметр строки запроса **expand** можно использовать со следующими свойствами навигации:

- страницы: **parentNotebook**, **parentSection**;
- разделы: **parentNotebook**, **parentSectionGroup**;
- группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;
- записные книжки: **sections**, **sectionGroups**.


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a>Информация о запросах *GET* и соответствующих ответах

| Данные запроса | Описание |  
|------|------|  
| Протокол | Все запросы используют протокол SSL/TLS для HTTPS. |  
| Заголовок Authorization | <p>`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</p><p>Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401. См. статью [Проверка подлинности и разрешения](permissions-reference.md).</p> |  
| Заголовок Accept | <p> `application/json` — для объектов OneNote и их наборов.</p><p> `text/html` — для содержимого страницы.</p> | 

<br/>

| Данные в отклике | Описание |  
|------|------|  
| Код успешного завершения | Код состояния HTTP 200 |  
| Текст ответа | Представление объекта или набора объектов в формате JSON, HTML-код страницы или двоичные данные файлового ресурса.  |  
| Ошибки | Если запрос завершается сбоем, API возвращает [ошибки](onenote-error-codes.md) в объекте **\@api.diagnostics** в тексте ответа. |  
| Заголовок X-CorrelationId | GUID, уникальный идентификатор запроса. Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт. |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a>Составление корневого URL-адреса для службы заметок Microsoft Graph

Для всех вызовов заметок Microsoft Graph используется следующий формат корневого URL-адреса:

`https://graph.microsoft.com/{version}/me/onenote/`  

Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph. Используйте значение `v1.0` для стабильного кода в рабочей среде. Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде. 

Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым). Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения ИД пользователей. 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a>Разрешения для запросов GET

Чтобы получить содержимое или структуру OneNote, необходимо запросить соответствующие разрешения. 

Указанные ниже разрешения позволяют выполнять запросы GET к Microsoft Graph. Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.

Варианты:

- Notes.read
- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).

<a name="see-also"></a>

## <a name="see-also"></a>См. также

- [Входной и выходной HTML-код для страниц OneNote](onenote-input-output-html.md)
- [Интеграция с OneNote](integrate-with-onenote.md)
- [Блог разработчиков OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»](/answers/topics/microsoft-graph-notes.html)
- [Репозитории GitHub OneNote](https://go.microsoft.com/fwlink/?LinkID=390178)