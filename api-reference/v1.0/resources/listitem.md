---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a>Ресурс ListItem

Этот ресурс представляет элемент объекта **[list][]** в SharePoint.
Значения столбцов в списке доступны через словарь `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Задачи для ресурса listItem

Ниже перечислены задачи, доступные для ресурсов **listItem**.
Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.

| Стандартная задача                    | Метод HTTP
|:-------------------------------|:------------------------
| [Получение][]                        | GET /items/{item-id}
| [Получение значений столбцов][Получение]       | GET /items/{item-id}?expand=fields
| [Создание][]                     | POST /items
| [Удаление][]                     | DELETE /items/{item-id}
| [Обновление][]                     | PATCH /items/{item-id}
| [Обновление значений столбцов][Обновление] | PATCH /items/{item-id}/fields

[Получение]: ../api/listItem_get.md
[Создание]: ../api/listItem_create.md
[Удаление]: ../api/listItem_delete.md
[Обновление]: ../api/listItem_update.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **listItem** в формате JSON.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **listItem**.

| Имя свойства | Тип                | Описание
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Тип контента для данного элемента списка.
| fields        | [fieldValueSet][]   | Значения столбцов, установленные для данного элемента списка.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип             | Описание
|:---------------------|:-----------------|:-----------------------------------
| id                   | string           | Уникальный идентификатор элемента. Только для чтения.
| name                 | string           | Имя или название элемента.
| createdBy            | [identitySet][]  | Удостоверение создателя данного элемента. Только для чтения.
| createdDateTime      | DateTimeOffset   | Дата и время создания элемента. Только для чтения.
| description          | строка           | Текст с описанием элемента.
| lastModifiedBy       | [identitySet][]  | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset   | Дата и время последнего изменения элемента. Только для чтения.
| webUrl               | строка (url-адрес)     | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

 Ниже перечислены связи ресурса **listItem** с другими ресурсами.

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:-------------------------------
| driveItem         | [driveItem][]               | Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
