---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: 2c98cb57bfd860b568b1cba95ed7f6fcf455eea1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564262"
---
# <a name="folder-resource-type"></a>Тип ресурса Folder

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
| **childCount** | Int32          | Количество дочерних элементов, содержащихся непосредственно в этом контейнере.
| **view**       | [folderView][] | Коллекция свойств, определяющих рекомендуемое представление для папки.

## <a name="remarks"></a>Замечания 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
