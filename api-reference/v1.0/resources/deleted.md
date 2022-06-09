---
author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
ms.localizationpriority: medium
description: Тип ресурса Deleted указывает, что элемент был удален.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 3ba5423b677455735323ea96738f56a7946ac200
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971268"
---
# <a name="deleted-facet"></a>Аспект Deleted

Пространство имен: microsoft.graph

Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.

Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                               |
|:---------|:-------|:------------------------------------------|
| state    | String | Представляет состояние удаленного элемента. |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->

