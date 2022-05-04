---
author: JeremyKelley
title: Тип ресурса site
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2eef3e7f3e46d28fe848b5693329e967c05a9a54
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191473"
---
# <a name="site-resource-type"></a>Тип ресурса site

Пространство имен: microsoft.graph

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
| [Отслеживание сайта][]          | коллекция сайтов | Отслеживание сайта пользователя или нескольких сайтов.
| [Прекращение отслеживания сайта][]        | коллекция сайтов | Отслеживание сайта пользователя или нескольких сайтов.
| [Перечисление отслеживаемых сайтов][]  | коллекция сайтов | Перечисление сайтов, отслеживаемых вошедшим пользователем.
| [Получение разрешения][]             | GET /sites/{site-id}/permissions/{permission-id}
| [Список разрешений][]           | GET /sites/{site-id}/permissions
| [Создание разрешений][]         | POST /sites/{site-id}/permissions
| [Удаление разрешения][]         | DELETE /sites/{site-id}/permissions/{permission-id}
| [Обновление разрешения][]         | PATCH /sites/{site-id}/permissions/{permission-id}
| [Операции со списком](../api/site-list-operations.md)|Коллекция [richLongRunningOperation](../resources/richlongrunningoperation.md)|Получите список [длительных операций](../resources/richlongrunningoperation.md) связанных с [сайтом](../resources/site.md).

[Получение сайта]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md
[Поиск сайтов]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md
[Отслеживание сайта]: ../api/site-follow.md
[Прекращение отслеживания сайта]: ../api/site-unfollow.md
[Перечисление отслеживаемых сайтов]: ../api/sites-list-followed.md
[Получение разрешения]: ../api/site-get-permission.md
[Список разрешений]: ../api/site-list-permissions.md
[Создание разрешений]: ../api/site-post-permissions.md
[Удаление разрешения]: ../api/site-delete-permission.md
[Обновление разрешения]: ../api/site-update-permission.md

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
| **root**                 | [root](root.md)                     | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения. |
| **webUrl**               | строка (url-адрес)                        | URL-адрес для отображения элемента в браузере. Только для чтения.                                          |

### <a name="id-property"></a>Свойство id
Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:
* имя узла семейства веб-сайтов (contoso.sharepoint.com);
* уникальный идентификатор семейства веб-сайтов (GUID);
* уникальный идентификатор сайта (GUID).
  
Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.

* `/sites/root`. Корневой сайт клиента.
* `/groups/{group-id}/sites/root`. Сайт группы для ресурса group.
  
## <a name="relationships"></a>Связи

| Связь      | Тип                                             | Описание
|:------------------|:-------------------------------------------------|:----------------------
| **analytics**     | Ресурс [itemAnalytics][]                       | Аналитические данные о действиях просмотра, выполненных на этом сайте.
| **columns**       | Collection([columnDefinition][])                 | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.
| **contentTypes**  | Collection([contentType][])                      | Коллекция типов контента, определенных для этого сайта.
| **drive**         | [drive][]                                        | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Collection([drive][])                            | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][])                         | Используется для адресации любого элемента на этом сайте. Перечисление этой коллекции невозможно.
| **lists**         | Collection([list][])                             | Коллекция списков на этом сайте.
| **onenote**       | [onenote][]                                      | Вызывает службу OneNote для выполнения операций, связанных с записными книжками.
| **operations**    | Коллекция [richLongRunningOperation](../resources/richlongrunningoperation.md) | Коллекция длительных операций на сайте.
| **permissions**   | Collection([permission][])                       | Разрешения, связанные с сайтом. Допускается значение NULL.
| **sites**         | Collection([site][])                             | Коллекция дочерних сайтов этого сайта.
| **termStore**     | [microsoft.graph.termStore.store]                | TermStore по умолчанию на этом сайте.
| **termStores**    | Коллекция[(microsoft.graph.termStore.store)]    | Коллекция termStores на этом сайте.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[site]: site.md
[onenote]: onenote.md
[microsoft.graph.termStore.store]: termstore-store.md

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

Ресурс **site** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "permissions",
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
  "operations": [ { "@odata.type": "microsoft.graph.richLongRunningOperation" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": { "@odata.type": "microsoft.graph.onenote"},
  "termStore": { "@odata.type": "microsoft.graph.termStore.store" },
  "termStores": [ { "@odata.type": "microsoft.graph.termStore.store" } ],

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
