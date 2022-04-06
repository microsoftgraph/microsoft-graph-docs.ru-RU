---
author: rahmit
description: Этот ресурс представляет страницу в списке SitePages.
ms.date: 03/15/2018
title: SitePage
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 981d6795a5c7999854e8c1ac55b7e9429622eabb
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723636"
---
# <a name="sitepage-resource"></a>ресурс sitePage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот ресурс представляет страницу в списке SitePages[.][]
Он содержит название, макет и коллекцию [webParts][].

## <a name="tasks-on-a-page"></a>Задачи на странице

Следующие задачи доступны для **ресурсов sitePage** .
Все примеры относительно [сайта;][] например, `https://graph.microsoft.com/{api-version}/sites/{site-id}`.

| Стандартная задача    | Метод HTTP                   |
| :------------- | :---------------------------- |
| [Перечисление страниц][] | GET /pages                    |
| [Вывод страницы][]   | GET /pages/{page-id}          |
| [Создание][]     | POST /pages                   |
| [Delete][]     | DELETE /pages/{page-id}       |
| [Публикация][]    | POST /pages/{page-id}/publish |

[Перечисление страниц]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **sitePage** .

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

Ресурс **sitePage** имеет следующие свойства.

| Свойство    | Тип                | Описание                   |
| :---------- | :------------------ | :---------------------------- |
| contentType | [contentTypeInfo][] | Тип контента страницы. |

## <a name="page-content"></a>Содержимое страницы

Ресурс **sitePage** имеет следующие поля контента.

| Имя свойства | Тип        | Описание                              |
| :------------ | :---------- | :--------------------------------------- |
| title         | string      | Заголовок страницы.                   |
| pageLayout    | строка      | Имя макета страницы. |
| webParts      | [webPart][] | Веб-части на странице.               |

## <a name="authoring-metadata"></a>Авторство метаданных

На **ресурсе sitePage** есть следующие метаданные, связанные с авторингом. Свойство **publishingState будет** отражать состояние авторинга страниц, как выехав или опубликованный.

| Имя свойства   | Тип                 | Описание                                              |
| :-------------- | :------------------- | :------------------------------------------------------- |
| publishingState | [publicationFacet][]. | Состояние публикации и MM.mm версии страницы. |

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание                                              |
| :------------------- | :---------------- | :------------------------------------------------------- |
| id                   | string            | Уникальный идентификатор элемента. Только для чтения.            |
| name                 | string            | Имя или название элемента.                            |
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.         |
| eTag                 | string            | ETag для элемента. Только для чтения.                            |
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.   |
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения. |
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Только для чтения. |
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.    |

## <a name="relationships"></a>Связи

Ресурс **sitePage** не имеет связей с другими ресурсами.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md.
[сайта]: site.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page&quot;: &quot;#"
  },
  "suppressions": []
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
