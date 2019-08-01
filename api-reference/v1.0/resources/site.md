---
author: JeremyKelley
ms.author: JeremyKelley
title: Ресурс site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 56df3754ab0fc87e839e3eb71db06ea5b05c75e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034176"
---
# <a name="site-resource"></a>Ресурс site

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="methods"></a>Методы

| Метод                | Тип возвращаемых данных | Описание
|:-------------------------|:-------------|:----------
| [Получение корневого сайта][]        | site | Получение доступа к корневому сайту SharePoint внутри клиента.
| [Получение сайта][]             | site | Получение доступа к сайту SharePoint с помощью параметра siteId.
| [Получение сайта по пути][]     | site | Получение доступа к корневому сайту SharePoint с использованием относительного пути.
| [Получение сайта для группы][] | site | Получение доступа к сайту группы для группы.
| [Получение аналитики][]              | [itemAnalytics][] | Получение аналитических данных для ресурса. 
| [Получение действий по интервалу][] | [itemActivityStat][] | Получение коллекции объектов **itemActivityStats** в пределах указанного интервала времени.
| [Поиск сайтов][]     | коллекция сайтов | Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.

[Получение сайта]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md
[Поиск сайтов]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md

## <a name="properties"></a>Свойства

| Свойство            | Тип                                | Описание                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | Уникальный идентификатор элемента. Только для чтения.                                                  |
| **createdDateTime**      | DateTimeOffset                      | Дата и время создания элемента. Только для чтения.                                             |
| **description**          | string                              | Текст с описанием сайта.                                                             |
| **displayName**          | string                              | Полное название сайта. Только для чтения.                                                        |
| **eTag**                 | string                              | ETag для элемента. Только для чтения.                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | Дата и время последнего изменения элемента. Только для чтения.                                       |
| **name**                 | string                              | Имя или название элемента.                                                                  |
| **root**                 | [root](root.md)                     | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения. |
| **webUrl**               | строка (url-адрес)                        | URL-адрес для отображения элемента в браузере. Только для чтения.                                          |

## <a name="relationships"></a>Связи

| Отношение      | Тип                             | Описание
|:------------------|:---------------------------------|:----------------------
| **analytics**     | Ресурс [itemAnalytics][]       | Аналитические данные о действиях просмотра, выполненных на этом сайте.
| **columns**       | Collection([columnDefinition][]) | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.
| **contentTypes**  | Collection([contentType][])      | Коллекция типов контента, определенных для этого сайта.
| **drive**         | [drive][]                        | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Collection([drive][])            | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][])         | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.
| **lists**         | Collection([list][])             | Коллекция списков на этом сайте.
| **sites**         | Collection([site][])             | Коллекция дочерних сайтов этого сайта.
| **onenote**       | [onenote][]                      | Вызывает службу OneNote для выполнения операций, связанных с записными книжками.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

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
