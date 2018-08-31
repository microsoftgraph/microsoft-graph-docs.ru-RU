---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: site
ms.openlocfilehash: 20d31a9cdc0e540c2b2f2d93fedabdc254e9c03e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265717"
---
# <a name="site-resource"></a>Ресурс site

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="tasks"></a>Задачи

Все приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.

| Имя задачи                | Пример запроса
|:-------------------------|:--------------------------------------------------
| [Получение корневого сайта][]        | GET /sites/root
| [Получение сайта][]             | GET /sites/{site-id}
| [Получение сайта по пути][]     | GET /sites/{hostname}:/{site-path}
| [Получение сайта для группы][] | GET /groups/{group-id}/sites/root
| [Поиск сайтов][]     | GET /sites?search={query}

[Получение сайта]: ../api/site_get.md
[Получение корневого сайта]: ../api/site_get.md
[Получение сайта по пути]: ../api/site_getbypath.md
[Получение сайта для группы]: ../api/site_get.md
[Поиск сайтов]: ../api/site_search.md

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

## <a name="properties"></a>Свойства

| Имя свойства            | Тип                                | Описание                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | Уникальный идентификатор элемента. Только для чтения.                                                  |
| **createdDateTime**      | DateTimeOffset                      | Дата и время создания элемента. Только для чтения.                                             |
| **description**          | string                              | Текст с описанием сайта.                                                             |
| **displayName**          | string                              | Полное название сайта. Только для чтения.                                                        |
| **eTag**                 | string                              | ETag для элемента. Только для чтения.                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | Дата и время последнего изменения элемента. Только для чтения.                                       |
| **name**                 | string                              | Имя или название элемента.                                                                  |
| **root**                 | [root](root.md)                     | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения. |
| **webUrl**               | строка (url-адрес)                        | URL-адрес для отображения элемента в браузере. Только для чтения.                                          |

## <a name="relationships"></a>Связи

| Имя связи | Тип                             | Описание
|:------------------|:---------------------------------|:----------------------
| **columns**       | Коллекция ([columnDefinition][]) | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.
| **contentTypes**  | Коллекция ([contentType][])      | Коллекция типов контента, определенных для этого сайта.
| **drive**         | [drive][]                        | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Коллекция([drive][])            | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][])         | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.
| **lists**         | Collection([list][])             | Коллекция списков на этом сайте.
| **sites**         | Коллекция([site][])             | Коллекция дочерних сайтов этого сайта.
| **onenote**       | [onenote][]                      | Вызывает службу OneNote для выполнения операций, связанных с записными книжками.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
