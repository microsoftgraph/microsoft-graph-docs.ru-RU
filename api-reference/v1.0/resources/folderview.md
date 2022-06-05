---
author: JeremyKelley
title: folderView
ms.localizationpriority: medium
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 79614af785392918026c857816505a12c9f8e476
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900165"
---
# <a name="folderview-resource-type"></a>Тип ресурса folderView

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

### <a name="sortby-options"></a>Параметры sortBy

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


### <a name="sortorder-options"></a>Параметры sortOrder

Для свойства **sortOrder** определены указанные ниже значения.

| Значение        | Описание
| ------------ | --------------------------------------------------------------
| `ascending`  | Элементы следует упорядочить по возрастанию.
| `descending` | Элементы следует упорядочить по убыванию.


### <a name="viewtype-options"></a>Параметры viewType

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

