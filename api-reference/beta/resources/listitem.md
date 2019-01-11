---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.openlocfilehash: b2e151937d5e8db633edeb5d521d6e0c875b6d78
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866089"
---
# <a name="listitem-resource"></a>Ресурс ListItem

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Этот ресурс представляет элемент объекта **[list][]** в SharePoint.
Значения столбцов в списке доступны через словарь `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Задачи для ресурса listItem

Ниже перечислены задачи, доступные для ресурсов **listItem**.
Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Стандартная задача                    | Метод HTTP
|:-------------------------------|:------------------------
| [Получение][]                        | GET /items/{item-id}
| [Получение значений столбцов][Получение]       | GET /items/{item-id}?expand=fields
| [Получение аналитики][]              | GET /items/ {идентификатор элемента} / аналитики
| [Получение действий по интервал][] | GET /items/ {идентификатор элемента} / getActivitiesByInterval
| [Создание][]                     | POST /items
| [Удаление][]                     | DELETE /items/{item-id}
| [Обновление][]                     | PATCH /items/{item-id}
| [Обновление значений столбцов][Обновление] | PATCH /items/{item-id}/fields

[Получение]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Создание]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **listItem** в формате JSON.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **listItem**.

| Имя свойства | Тип                | Описание
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Тип контента для данного элемента списка.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | строка            | Уникальный идентификатор элемента. Только для чтения.
| name                 | строка            | Имя или название элемента.
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.
| createdDateTime      | DateTimeOffset    | Дата и время создания элемента. Только для чтения.
| description          | строка            | Текст с описанием элемента.
| eTag                 | string            | ETag для элемента. Только для чтения.                                                          |
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.
| sharepointIds        | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

 Ниже перечислены связи ресурса **listItem** с другими ресурсами.

| Имя связи | Тип                           | Описание
|:------------------|:-------------------------------|:-------------------------------
| activities        | Коллекция [itemActivity][]    | Список последних действий, выполненных с элементом.
| Аналитика         | [itemAnalytics][] ресурсов     | Аналитика о Просмотр действий, выполняемых по этому элементу.
| driveItem         | [driveItem][]                  | Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**
| fields            | [fieldValueSet][]              | Значения столбцов, установленные для данного элемента списка.
| версии          | [listItemVersion][] коллекции | Список предыдущих версий элемента списка.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[списки]: list.md
[listItemVersion]: listitemversion.md.
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
