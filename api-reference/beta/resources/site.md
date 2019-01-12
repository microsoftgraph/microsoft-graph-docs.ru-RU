---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1676a314b7c1283918518655b3180cbc70ca193e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952351"
---
# <a name="site-resource-type"></a>Тип ресурса сайта

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="methods"></a>Методы

| Метод                         | Путь REST
|:-------------------------------|:--------------------------------------------
| [Получение корневого сайта][]              | GET /sites/root
| [Получение сайта][]                   | GET /sites/{site-id}
| [Получение сайта по пути][]           | GET /sites/{hostname}:/{site-path}
| [Получение сайта для группы][]       | GET /groups/{group-id}/sites/root
| [Получение аналитики][]              | GET/Sites / {идентификатор сайта} / аналитики
| [Получение действий по интервал][] | GET/Sites / {идентификатор сайта} / getActivitiesByInterval
| [Перечисление страниц][]                 | GET/Sites / {идентификатор сайта} / pages
| [Узлы корневого списка][]            | / Sites GET? фильтра = ne корневой значение null и выделить = siteCollection, webUrl
| [Поиск сайтов][]           | GET /sites?search={query}

[Получение сайта]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Перечисление страниц]: ../api/sitepage-list.md
[Узлы корневого списка]: ../api/site-list.md
[Поиск сайтов]: ../api/site-search.md


## <a name="properties"></a>Свойства

| Имя свойства            | Тип               | Описание
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | строка             | Уникальный идентификатор элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset     | Дата и время создания элемента. Только для чтения.
| **description**          | строка             | Текст с описанием сайта.
| **eTag**;                 | string             | ETag для элемента. Только для чтения.                                                                  |
| **displayName**          | строка             | Полное название сайта. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset     | Дата и время последнего изменения элемента. Только для чтения.
| **name**                 | строка             | Имя или название элемента.
| **root**                 | [root][]           | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.
| **sharepointIds**        | [sharepointIds][]  | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| **siteCollection**       | [siteCollection][] | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.
| **webUrl**               | строка (url-адрес)       | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

| Имя связи | Тип                             | Описание
|:------------------|:---------------------------------|:----------------------
| **Аналитика**     | [itemAnalytics][] ресурсов       | Аналитика о Просмотр действий, выполняемых на данном сайте.
| **columns**       | Коллекция ([columnDefinition][]) | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.
| **contentTypes**  | Коллекция ([contentType][])      | Коллекция типов контента, определенных для этого сайта.
| **drive**         | [drive][]                        | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Collection([drive][])            | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][])         | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.
| **lists**         | Collection([list][])             | Коллекция списков на этом сайте.
| **страницы**         | Коллекции ([sitePage][])         | Набор страниц в списке SitePages на данном сайте.
| **sites**         | Collection([site][])             | Коллекция дочерних сайтов этого сайта.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[списки]: list.md
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
