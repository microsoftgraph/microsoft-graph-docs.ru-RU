---
author: JeremyKelley
ms.date: 09/11/2017
title: Перечисление
ms.localizationpriority: high
ms.prod: sharepoint
description: Ресурс list представляет список на сайте.
doc_type: resourcePageType
ms.openlocfilehash: 9d47d308ffa1171ff720d66f7ed21f254b5ec06b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021500"
---
# <a name="list-resource"></a>Ресурс List

Пространство имен: microsoft.graph

Ресурс **list** представляет список в ресурсе [site][].
Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.

## <a name="tasks-on-a-list"></a>Задачи для ресурса list

Ниже перечислены задачи, доступные для ресурсов list.
**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.
Однако вы можете создавать и менять [элементы списков][listItem].

Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/v1.0/sites/{site-id}`.

| Стандартная задача               | Метод HTTP
|:--------------------------|:------------------------------
| [Получение списка][]              | GET /lists/{list-id}
| [Создание списка][]           | POST /lists
| [Перечисление элементов списка][]  | GET /lists/{list-id}/items
| [Обновление элемента списка][]      | PATCH /lists/{list-id}/items/{item-id}
| [Удаление элемента списка][]      | DELETE /lists/{list-id}/items/{item-id}
| [Создание элемента в списке][]      | POST /lists/{list-id}
| [Получение канала WebSocket][] | GET /lists/{list-id}/subscriptions/socketIo

[Получение списка]: ../api/list-get.md
[Создание списка]: ../api/list-create.md
[Перечисление элементов списка]: ../api/listitem-list.md
[Обновление элемента списка]: ../api/listitem-update.md
[Удаление элемента списка]: ../api/listitem-delete.md
[Создание элемента в списке]: ../api/listitem-create.md
[Получение канала WebSocket]: ../api/subscriptions-socketio.md

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **list** в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template&quot;: &quot;documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
  },
  "system": false,
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl&quot;: &quot;url to visit the list in a browser"
}
```

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **list**.

| Имя свойства    | Тип                             | Описание
|:-----------------|:---------------------------------|:---------------------------
| **displayName**  | строка                           | Отображаемый заголовок списка.
| **list**         | [listInfo][]                     | Предоставляет дополнительные сведения о списке.
| **system**       | [systemFacet][]                  | Если это свойство задано, оно указывает, что данным списком управляет система. Только для чтения.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства            | Тип              | Описание
|:-------------------------|:------------------|:------------------------------
| **id**                   | string            | Уникальный идентификатор элемента. Только для чтения.
| **name**                 | строка            | Имя элемента.
| **createdBy**            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset    | Дата и время создания элемента. Только для чтения.
| **description**          | строка            | Текст с описанием элемента.
| **eTag**                 | string            | ETag для элемента. Только для чтения.                                                          |
| **lastModifiedBy**;       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.
| **parentReference**      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.
| **sharepointIds**        | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| **webUrl**               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

Ниже перечислены связи ресурса **list** с другими ресурсами.

| Имя связи | Тип                             | Описание
|:------------------|:---------------------------------|:----------------------
| **drive**         | [drive][]                        | Доступна только для библиотек документов. Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].
| **items**         | Коллекция ([listItem][])         | Все элементы, содержащиеся в списке.
| **columns**       | Коллекция ([columnDefinition][]) | Коллекция определений полей для данного списка.
| **contentTypes**  | Коллекция ([contentType][])      | Коллекция типов контента в данном списке.
| **subscriptions** | Коллекция ([subscription][])     | Набор подписок на список.

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md
[subscription]: subscription.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists&quot;: &quot;#"
  }
} -->

