---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643764"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса networkLocationDetail
Указывает сведения, связанные с сетевую папку. .



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|networkType|String|Предоставляет тип сети. Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.|
|networkName|String|Имя сети.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
