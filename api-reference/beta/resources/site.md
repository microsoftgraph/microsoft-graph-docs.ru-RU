---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
title: Тип ресурса site
ms.localizationpriority: high
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 423986ac43de3558836660a1684978784db724eb
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059976"
---
# <a name="site-resource-type"></a>Тип ресурса site

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="methods"></a>Методы

| Метод                                            | Путь REST                                                   |
| :------------------------------------------------ | :---------------------------------------------------------- |
| [Получение корневого сайта][]                                 | GET /sites/root                                             |
| [Получение сайта][]                                      | GET /sites/{site-id}                                        |
| [Получение сайта по пути][]                              | GET /sites/{hostname}:/{site-path}                          |
| [Получение сайта для группы][]                          | GET /groups/{group-id}/sites/root                           |
| [Получение аналитики][]                                 | GET /sites/{site-id}/analytics                              |
| [Получение действий по интервалу][]                    | GET /sites/{site-id}/getActivitiesByInterval                |
| [Перечисление страниц][]                                    | GET /sites/{site-id}/pages                                  |
| [Перечисление корневых сайтов][]                               | GET /sites?filter=root ne null&select=siteCollection,webUrl |
| [Поиск сайтов][]                              | GET /sites?search={query}                                   |
| [Отслеживание сайта][]                                   | POST /users/{user-id}/followedSites/add                     |
| [Прекращение отслеживания сайта][]                                 | POST /users/{user-id}/followedSites/remove                  |
| [Перечисление отслеживаемых сайтов][]                           | GET /me/followedSites                                       |
| [Получение разрешения][]                                | GET /sites/{site-id}/permissions/{permission-id}            |
| [Список разрешений][]                              | GET /sites/{site-id}/permissions                            |
| [Создание разрешений][]                            | POST /sites/{site-id}/permissions                           |
| [Удаление разрешения][]                             | DELETE /sites/{site-id}/permissions/{permission-id}         |
| [Обновление разрешения][]                             | PATCH /sites/{site-id}/permissions/{permission-id}          |
| [Перечисление типов контента][]                            | GET /sites/{site-id}/contentTypes                           |
| [Создание contentType][]                            | POST /sites/{site-id}/contentTypes                          |
| [Перечисление столбцов][]                                  | GET /sites/{site-id}/columns                                |
| [Создание столбца][]                                 | POST /sites/{site-id}/columns                               |
| [Операции со списком](../api/site-list-operations.md) | GET /sites/{site-id}/operations                             |
| [Получение параметров сайта][]                             | GET /sites/{site-id}/settings                               |

[Получение сайта]: ../api/site-get.md
[Получение корневого сайта]: ../api/site-get.md
[Получение сайта по пути]: ../api/site-getbypath.md
[Получение сайта для группы]: ../api/site-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Перечисление страниц]: ../api/sitepage-list.md
[Перечисление корневых сайтов]: ../api/site-list.md
[Поиск сайтов]: ../api/site-search.md
[Отслеживание сайта]: ../api/site-follow.md
[Прекращение отслеживания сайта]: ../api/site-unfollow.md
[Перечисление отслеживаемых сайтов]: ../api/sites-list-followed.md
[Получение разрешения]: ../api/site-get-permission.md
[Список разрешений]: ../api/site-list-permissions.md
[Создание разрешений]: ../api/site-post-permissions.md
[Удаление разрешения]: ../api/site-delete-permission.md
[Обновление разрешения]: ../api/site-update-permission.md
[Перечисление типов контента]: ../api/site-list-contenttypes.md
[Создание contentType]: ../api/site-post-contenttypes.md
[Перечисление столбцов]: ../api/site-list-columns.md
[Создание столбца]: ../api/site-post-columns.md
[Получение параметров сайта]: ../api/sitesettings-get.md

## <a name="properties"></a>Свойства

| Свойство                 | Тип               | Описание                                                                                    |
| :----------------------- | :----------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string             | [Уникальный идентификатор](#id-property) элемента. Только для чтения.                                  |
| **createdDateTime**      | DateTimeOffset     | Дата и время создания элемента. Только для чтения.                                             |
| **description**          | string             | Текст с описанием сайта.                                                             |
| **eTag**                 | string             | ETag для элемента. Только для чтения.                                                                  |
| **displayName**          | string             | Полное название сайта. Только для чтения.                                                        |
| **lastModifiedDateTime** | DateTimeOffset     | Дата и время последнего изменения элемента. Только для чтения.                                       |
| **name**                 | string             | Имя или название элемента.                                                                  |
| **root**                 | [root][]           | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.            |
| **settings**             | [siteSettings]     | Параметры на этом сайте. Только для чтения.                                |
| **sharepointIds**        | [sharepointIds][]  | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                       |
| **siteCollection**       | [siteCollection][] | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения. |
| **webUrl**               | строка (url-адрес)       | URL-адрес для отображения элемента в браузере. Только для чтения.                                          |

### <a name="id-property"></a>Свойство id

Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:
* имя узла семейства веб-сайтов (contoso.sharepoint.com);
* уникальный идентификатор семейства веб-сайтов (GUID);
* уникальный идентификатор сайта (GUID).

Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.

* `/sites/root`. Корневой сайт клиента.
* `/groups/{group-id}/sites/root`. Сайт группы для ресурса group.

## <a name="relationships"></a>Связи

| Связь        | Тип                                                                            | Описание                                                                                                                                |
| :------------------ | :------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| **analytics**       | Ресурс [itemAnalytics][]                                                      | Аналитические данные о действиях просмотра, выполненных на этом сайте.                                                                          |
| **columns**         | Collection([columnDefinition][])                                                | Коллекция определений столбцов, которые можно повторно использовать в разных списках на этом сайте.                                                                |
| **contentTypes**    | Collection([contentType][])                                                     | Коллекция типов контента, определенных для этого сайта.                                                                                     |
| **drive**           | [drive][]                                                                       | Диск по умолчанию (библиотека документов) для этого сайта.                                                                                        |
| **drives**          | Collection([drive][])                                                           | Коллекция дисков (библиотек документов) на этом сайте.                                                                             |
| **items**           | Collection([baseItem][])                                                        | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.                                                     |
| **lists**           | Collection([list][])                                                            | Коллекция списков на этом сайте.                                                                                                   |
| **operations**      | Коллекция [richLongRunningOperation](../resources/richlongrunningoperation.md) | Коллекция длительных операций для сайта.                                                                                    |
| **pages**           | Collection([sitePage][])                                                        | Коллекция страниц в списке SitePages на этом сайте.                                                                                |
| **permissions**     | Collection([permission][])                                                      | Разрешения, связанные с сайтом. Допускается значение NULL.                                                                                        |
| **sites**           | Collection([site][])                                                            | Коллекция дочерних сайтов этого сайта.                                                                                           |
| **termStore**       | [microsoft.graph.termStore.store]                                               | TermStore на этом сайте.                                                                                                             |
| **externalColumns** | Collection([columnDefinition][])                                                | Коллекция определений столбцов, доступных на сайте, на которые ссылаются сайты в родительской иерархии текущего сайта. |

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[siteSettings]: sitesettings.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md
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
  "displayName": "string",
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "settings": { "@odata.type": "microsoft.graph.sitesettings" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "termStore": { "@odata.type": "microsoft.graph.termStore.store" },

  /* inherited from baseItem */
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "name": "string",
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
  "suppressions": []
}
-->
