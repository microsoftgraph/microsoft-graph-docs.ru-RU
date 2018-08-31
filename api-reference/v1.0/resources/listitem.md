---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 13ddb00d90880570361c7dcbe198c7c90e044957
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264401"
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
| contentType   | [contentTypeInfo][] | Тип содержимого для данного элемента списка.

Следующие свойства наследуются от **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | string (строка)            | Уникальный идентификатор элемента. Только для чтения.
| name                 | string (строка)            | Имя или название элемента.
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.
| createdDateTime      | DateTimeOffset    | Дата и время создания элемента. Только для чтения.
| description          | string (строка)            | Текст с описанием элемента.
| eTag                 | string (строка)            | ETag для элемента. Только для чтения.                                                          |
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.
| parentReference      | [itemReference][] | Сведения о родительском элементе, если у элемента таковой имеется. Чтение и запись.
| sharepointIds        | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

 Ниже перечислены связи ресурса **listItem** с другими ресурсами.

| Имя связи | Тип                           | Описание
|:------------------|:-------------------------------|:-------------------------------
| driveItem         | [driveItem][]                  | Для библиотек документов связь **driveItem** предоставляет listItem как **[driveItem][]**
| fields            | [fieldValueSet][]              | Значения столбцов, установленные для данного элемента списка.
| versions          | Коллекция [listItemVersion][] | Список предыдущих версий элемента списка.

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listItemVersion.md
[sharepointIds]: sharepointIds.md

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
