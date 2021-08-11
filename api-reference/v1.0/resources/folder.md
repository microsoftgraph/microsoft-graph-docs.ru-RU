---
author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'Ресурс Folder — это единая структура, объединяющая данные элемента, связанные с папками. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8160e90124d2e614c46a1aa87ad7d78900181b7ef6ee80e25e8083b1490515a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189746"
---
# <a name="folder-resource-type"></a>Тип ресурса Folder

Пространство имен: microsoft.graph

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
  "tocPath&quot;: &quot;Facets/Folder"
} -->

