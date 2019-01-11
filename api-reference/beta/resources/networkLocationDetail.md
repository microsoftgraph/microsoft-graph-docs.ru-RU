---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834323"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса networkLocationDetail
Указывает сведения, связанные с сетевую папку. .



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|networkType|Строка|Предоставляет тип сети. Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.|
|networkName|Строка|Имя сети.|


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
