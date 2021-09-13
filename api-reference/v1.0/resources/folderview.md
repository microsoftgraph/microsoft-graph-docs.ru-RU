---
author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
ms.localizationpriority: medium
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 72371634e8cebba4c520277de6bae7055a63ea97
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078849"
---
# <a name="folderview-resource-type"></a>Тип ресурса FolderView

Пространство имен: microsoft.graph

Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.

Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a>Свойства

| Имя свойства         | Тип   | Описание
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | строка | Метод сортировки содержимого папки.
| **sortOrder**         | строка | Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.
| **viewType**          | строка | Тип представления, который следует использовать для представления папки.

Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.

### <a name="sortby-options"></a>параметры sortBy

Для свойства **sortBy** определены указанные ниже значения.

| Значение                    | Описание
| ------------------------ | --------------------------------------------------
| `default`                | Порядок сортировки, используемый по умолчанию, в приложении.
| `name`                   | Элементы следует упорядочить по их свойству **name**.
| `type`                   | Элементы следует упорядочить по их типам.
| `size`                   | Элементы следует упорядочить по их свойству **size**.
| `takenOrCreatedDateTime` | Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.
| `lastModifiedDateTime`   | Элементы следует упорядочить по их свойству **lastModifiedDateTime**.
| `sequence`               | Для элементов используется настраиваемая последовательность, указанная пользователем.


### <a name="sortorder-options"></a>параметры sortOrder

Для свойства **sortOrder** определены указанные ниже значения.

| Значение        | Описание
| ------------ | --------------------------------------------------------------
| `ascending`  | Элементы следует упорядочить по возрастанию.
| `descending` | Элементы следует упорядочить по убыванию.


### <a name="viewtype-options"></a>параметры viewType

Для свойства **viewType** определены указанные ниже значения.

| Значение        | Описание
| ------------ | --------------------------------------------------------------
| `default`    | Тип представления, используемый по умолчанию, для приложения.
| `icons`      | Представление, в котором для представления элементов driveItems используются значки.
| `details`    | Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.
| `thumbnails` | Представление, в котором для представления элементов используются большие эскизы элементов driveItems.


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->

