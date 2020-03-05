---
author: JeremyKelley
description: Ресурс list представляет список на сайте.
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a7e59cf2e81371428e3816acc6e89c4a102ca40e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522962"
---
# <a name="list-resource"></a>Ресурс List

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **list** представляет список в ресурсе [site][].
Этот ресурс содержит высокоуровневые свойства списка, включая определения шаблонов и полей.

## <a name="tasks-on-a-list"></a>Задачи для ресурса list

Ниже перечислены задачи, доступные для ресурсов list.
**Примечание.** В этой бета-версии разрешается только навигация по спискам. Их создание и обновление не поддерживаются.
Однако вы можете создавать и менять [элементы списков][listItem].

Все приведенные ниже примеры относятся к сайту, например `https://graph.microsoft.com/beta/sites/{site-id}`.

| Стандартная задача               | Метод HTTP
|:--------------------------|:------------------------------
| [Получение списка][]              | GET /lists/{list-id}
| [Создание списка][]           | POST /lists
| [Перечисление элементов списка][]  | GET /lists/{list-id}/items
| [Обновление элемента списка][]      | PATCH /lists/{list-id}/items/{item-id}
| [Удаление элемента списка][]      | DELETE /lists/{list-id}/items/{item-id}
| [Создание элемента в списке][]      | POST /lists/{list-id}
| [Получение последних действий][] | GET /lists/{list-id}/activities
| [Получение канала WebSocket][] | ПОЛУЧЕНИЕ/Листс/{лист-ИД}/субскриптионс/соккетио

[Получение списка]: ../api/list-get.md
[Создание списка]: ../api/list-create.md
[Перечисление элементов списка]: ../api/listitem-list.md
[Обновление элемента списка]: ../api/listitem-update.md
[Удаление элемента списка]: ../api/listitem-delete.md
[Создание элемента в списке]: ../api/listitem-create.md
[Получение последних действий]: ../api/activities-list.md
[Получение канала WebSocket]: ../api/driveitem-subscriptions-socketio.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **list** в формате JSON.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **list**.

| Имя свойства    | Тип                             | Описание
|:-----------------|:---------------------------------|:---------------------------
| **columns**      | Коллекция ([columnDefinition][]) | Коллекция определений полей для данного списка.
| **contentTypes** | Коллекция ([contentType][])      | Коллекция типов контента в данном списке.
| **displayName**  | строка                           | Отображаемый заголовок списка.
| **list**         | [listInfo][]                     | Предоставляет дополнительные сведения о списке.
| **system**       | [systemFacet][]                  | Если это свойство задано, оно указывает, что данным списком управляет система. Только для чтения.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства            | Тип             | Описание
|:-------------------------|:-----------------|:-------------------------------
| **id**                   | строка           | Уникальный идентификатор элемента. Только для чтения.
| **name**                 | string           | Имя элемента.
| **createdBy**            | [identitySet][]  | Удостоверение создателя данного элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset   | Дата и время создания элемента. Только для чтения.
| **description**          | строка           | Текст с описанием элемента.
| **lastModifiedBy**;       | [identitySet][]  | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset   | Дата и время последнего изменения элемента. Только для чтения.
| **webUrl**               | строка (url-адрес)     | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

Ниже перечислены связи ресурса **list** с другими ресурсами.

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:------------------------------
| **activities**    | Коллекция [itemActivity][] | Последние действия, выполненные в списке.
| **drive**         | [drive][]                   | Доступна только для библиотек документов. Разрешает доступ к списку как к ресурсу [drive][] с объектами [driveItem][driveItem].
| **items**         | Коллекция ([listItem][])    | Все элементы, содержащиеся в списке.
| subscriptions      | Коллекция [subscription][] | Набор подписок в списке.

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[site]: site.md
[systemFacet]: systemfacet.md
[subscription]: subscription.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": []
}
-->
