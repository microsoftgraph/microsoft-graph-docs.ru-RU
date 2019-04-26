---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: 77c13d980590e908de5c7f0a8a7cbf67d1cf031e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340254"
---
# <a name="folder-resource-type"></a>Тип ресурса Folder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип           | Описание
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int64          | Количество дочерних элементов, содержащихся непосредственно в этом контейнере.
| **view**       | [folderView][] | Коллекция свойств, определяющих рекомендуемое представление для папки.


## <a name="remarks"></a>Замечания 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
