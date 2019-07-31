---
title: Тип ресурса Чанжетраккедентити
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3815b22c7bd76a894df0e98415e0c30bb77decd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974059"
---
# <a name="changetrackedentity-resource-type"></a>Тип ресурса Чанжетраккедентити

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime| DateTimeOffset| |
|lastModifiedDateTime| DateTimeOffset| |
|lastModifiedBy| [identitySet](identityset.md) | |

## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType":"microsoft.graph.entity",
  "abstract":true
}-->

``` json
{
    "createdDateTime":"String (timestamp)",
    "lastModifiedDateTime" :"String (timestamp)",
    "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```



