---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 6a51d858f529e65820d7bc55bb7ec8fec80186d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024823"
---
# <a name="deleted-facet"></a>Аспект Deleted

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
