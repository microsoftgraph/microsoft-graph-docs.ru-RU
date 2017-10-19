---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a>Ресурс List

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
| [Перечисление элементов списка][]  | GET /lists/{list-id}/items
| [Обновление элемента списка][]      | PATCH /lists/{list-id}/items/{item-id}
| [Удаление элемента списка][]      | DELETE /lists/{list-id}/items/{item-id}
| [Создание элемента в списке][]      | POST /lists/{list-id}

[Получение списка]: ../api/list_get.md
[Перечисление элементов списка]: ../api/listitem_list.md
[Обновление элемента списка]: ../api/listItem_update.md
[Удаление элемента списка]: ../api/listItem_delete.md
[Создание элемента в списке]: ../api/listItem_create.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **list** в формате JSON.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,

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
| **id**                   | string           | Уникальный идентификатор элемента. Только для чтения.
| **name**                 | строка           | Имя элемента.
| **createdBy**            | [identitySet][]  | Удостоверение создателя данного элемента. Только для чтения.
| **createdDateTime**      | DateTimeOffset   | Дата и время создания элемента. Только для чтения.
| **description**          | строка           | Текст с описанием элемента.
| **lastModifiedBy**       | [identitySet][]  | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| **lastModifiedDateTime** | DateTimeOffset   | Дата и время последнего изменения элемента. Только для чтения.
| **webUrl**               | строка (url-адрес)     | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

Ниже перечислены связи ресурса **list** с другими ресурсами.

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:------------------------------
| **drive**         | [drive][]                   | Доступна только для библиотек документов. Разрешает доступ к списку как к ресурсу [drive][] с ресурсами [driveItem][driveItem].
| **items**         | Коллекция ([listItem][])    | Все элементы, содержащиеся в списке.

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->
