---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: 65fc0a6aa702e6cd08f18dc16957bb7a41589f40
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="folderview-resource-type"></a>Тип ресурса FolderView

Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.

Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
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

### <a name="sortby-values"></a>Значения свойства sortBy

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


### <a name="sortorder-values"></a>Значения свойства sortOrder

Для свойства **sortOrder** определены указанные ниже значения.

| Значение        | Описание
| ------------ | --------------------------------------------------------------
| `ascending`  | Элементы следует упорядочить по возрастанию.
| `descending` | Элементы следует упорядочить по убыванию.


### <a name="viewtype-values"></a>Значения свойства viewType

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
  "tocPath": "Facets/FolderView"
} -->
