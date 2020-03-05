---
author: JeremyKelley
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7ad664b20f125857943e93e62b66301c82af89ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497869"
---
# <a name="folderview-resource-type"></a>Тип ресурса FolderView

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.

Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
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

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
