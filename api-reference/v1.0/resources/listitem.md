---
author: JeremyKelley
title: Ресурс listItem
description: Представляет элемент объекта list в SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 851b506b029d05bfac2bcecfcce57d9e3ce8684f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021465"
---
# <a name="listitem-resource"></a>Ресурс listItem

Пространство имен: microsoft.graph

Представляет элемент объекта [list][] в SharePoint.

Все элементы в библиотеке документов SharePoint могут быть представлены как ресурс **listItem** или [driveItem][].

Значения столбцов в списке доступны через словарь `fieldValueSet`.

## <a name="methods"></a>Методы

Ниже перечислены методы, доступные для ресурсов **listItem**.
Все примеры относятся к объекту **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.

| Метод                    | Возвращаемый тип | Описание
|:-------------------------------|:-------------------|:------
| [получение][];                   | listItem| Получение элемента списка.
| [Получение значений столбцов][Получение]       | listItem | Получение значений столбцов из ресурса listItem.
| [Получение аналитики][]              | [itemAnalytics][]| Получение аналитических данных для ресурса. 
| [Получение действий по интервалу][] | [itemActivityStat][]| Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.
| [Создание][]                     | listItem | Создание ресурса listItem в списке.
| [Удаление][]                     | Содержимое отсутствует | Удаление элемента из списка.
| [Обновление][]                     | [fieldValueSet][]| Изменение свойств ресурса listItem.
| [Обновление значений столбцов][Обновление] | [fieldValueSet][]| Изменение значений столбцов ресурса listItem.

[Получение]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md
[Создание]: ../api/listitem-create.md
[Удаление]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **listItem**.

| Имя свойства | Тип                | Описание
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Тип контента для данного элемента списка.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | string            | Уникальный идентификатор элемента. Только для чтения.
| name                 | string            | Имя или название элемента.
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
| analytics         | Ресурс [itemAnalytics][]     | Аналитические данные о действиях просмотра, выполненных для элемента.
| driveItem         | [driveItem][]                  | Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]**
| fields            | [fieldValueSet][]              | Значения столбцов, установленные для данного элемента списка.
| versions          | Коллекция [listItemVersion][] | Список предыдущих версий элемента списка.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **listItem** в формате JSON.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
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
  "webUrl&quot;: &quot;url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem&quot;: &quot;#"
  }
} -->

