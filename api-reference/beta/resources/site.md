---
author: JeremyKelley
description: Ресурс site предоставляет метаданные и связи для сайта SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 587014aa0c9dbe4c05c0e3b946c3f6e44b7cb821
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442802"
---
# <a name="site-resource-type"></a>Тип ресурса site

Пространство имен: microsoft.graph

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
| [Отслеживание сайта][]                | POST /users/{user-id}/followedSites/add
| [Прекращение отслеживания сайта][]              | POST /users/{user-id}/followedSites/remove
| [Перечисление отслеживаемых сайтов][]        | GET /me/followedSites
| [Получение разрешения][]             | GET /sites/{site-id}/permissions/{permission-id}
| [Список разрешений][]           | GET /sites/{site-id}/permissions
| [Создание разрешений][]         | POST /sites/{site-id}/permissions
| [Удаление разрешения][]         | DELETE /sites/{site-id}/permissions/{permission-id}
| [Обновление разрешения][]         | PATCH /sites/{site-id}/permissions/{permission-id}

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


## <a name="properties"></a>Свойства

| Имя свойства            | Тип               | Описание
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | string             | [Уникальный идентификатор](#id-property) элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset     | Дата и время создания элемента. Только для чтения.
| **description**          | string             | Текст с описанием сайта.
| **eTag**                 | string             | ETag для элемента. Только для чтения.                                                                  |
| **displayName**          | string             | Полное название сайта. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset     | Дата и время последнего изменения элемента. Только для чтения.
| **name**                 | string             | Имя или название элемента.
| **root**                 | [root][]           | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.
| **sharepointIds**        | [sharepointIds][]  | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| **siteCollection**       | [siteCollection][] | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения.
| **webUrl**               | string (url-адрес)       | URL-адрес для отображения элемента в браузере. Только для чтения.

### <a name="id-property"></a>Свойство id
Ресурс **site** идентифицируется посредством уникального идентификатора, при создании которого используются следующие значения:
* имя узла семейства веб-сайтов (contoso.sharepoint.com);
* уникальный идентификатор семейства веб-сайтов (GUID);
* уникальный идентификатор сайта (GUID).
  
Идентификатор `root` всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.

* `/sites/root`. Корневой сайт клиента.
* `/groups/{group-id}/sites/root`. Сайт группы для ресурса group.

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
| **permissions**   | Collection([permission][])         | Разрешения, связанные с сайтом. Допускается значение NULL.
| **sites**         | Collection([site][])             | Коллекция дочерних сайтов этого сайта.
| **externalColumns**     | Collection([columnDefinition][])  | Коллекция определений столбцов, доступных на сайте, на которые ссылаются сайты в родительской иерархии текущего сайта.

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
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
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
  "suppressions": []
}
-->
