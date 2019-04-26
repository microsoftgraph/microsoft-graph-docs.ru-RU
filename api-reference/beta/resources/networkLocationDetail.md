---
title: Тип ресурса Нетворклокатиондетаил
description: Показывает сведения, связанные с сетевым расположением. .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342179"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса Нетворклокатиондетаил
Показывает сведения, связанные с сетевым расположением.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Нетворктипе|Нетворктипе|Предоставляет тип сети. `intranet`Возможные значения: `extranet`, `namedNetwork`, и. `trusted`|
|Нетворкнамес|Коллекция String|Имена сетей.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
