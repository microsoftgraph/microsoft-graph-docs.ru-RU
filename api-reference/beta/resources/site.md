---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d2fbdcb870d86efb983de1e3ba75154b6e15f619
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481862"
---
# <a name="site-resource-type"></a>Тип ресурса site

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="methods"></a>Методы

| Метод                         | Путь REST
|:-------------------------------|:--------------------------------------------
| [Получение корневого сайта][]              | GET /sites/root
| [Получение сайта][]                   | GET /sites/{site-id}
| [Получение сайта по пути][]           | GET /sites/{hostname}:/{site-path}
| [Получение сайта для группы][]       | GET /groups/{group-id}/sites/root
| [Получение аналитики][]              | GET /sites/{site-id}/analytics
| [Получение действий по интервалу][] | GET /sites/{site-id}/getActivitiesByInterval
| [Перечисление страниц][]                 | GET /sites/{site-id}/pages
| [Перечисление корневых сайтов][]            | GET /sites?filter=root ne null&select=siteCollection,webUrl
| [Поиск сайтов][]           | GET /sites?search={query}

[Получение сайта]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Перечисление страниц]: ../api/sitepage-list.md
[Перечисление корневых сайтов]: ../api/site-list.md
[Поиск сайтов]: ../api/site-search.md


## <a name="properties"></a>Свойства

| Имя свойства            | Тип               | Описание
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | string             | Уникальный идентификатор элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset     | Дата и время создания элемента. Только для чтения.
| **description**          | string             | Текст с описанием сайта.
| **eTag**                 | string             | ETag для элемента. Только для чтения.                                                                  |
| **displayName**          | string             | Полное название сайта. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset     | Дата и время последнего изменения элемента. Только для чтения.
| **name**                 | string             | Имя или название элемента.
| **root**                 | [root][]           | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.
| **sharepointIds**        | [sharepointIds][]  | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| **siteCollection**       | [siteCollection][] | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.
| **webUrl**               | строка (url-адрес)       | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

| Имя связи | Тип                             | Описание
|:------------------|:---------------------------------|:----------------------
| **analytics**     | Ресурс [itemAnalytics][]       | Аналитические данные о действиях просмотра, выполненных на этом сайте.
| **columns**       | Collection([columnDefinition][]) | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.
| **contentTypes**  | Collection([contentType][])      | Коллекция типов контента, определенных для этого сайта.
| **drive**         | [drive][]                        | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Collection([drive][])            | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][])         | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.
| **lists**         | Collection([list][])             | Коллекция списков на этом сайте.
| **pages**         | Collection([sitePage][])         | Коллекция страниц в списке SitePages на этом сайте.
| **sites**         | Collection([site][])             | Коллекция дочерних сайтов этого сайта.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **site** в формате JSON.

Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/site.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
