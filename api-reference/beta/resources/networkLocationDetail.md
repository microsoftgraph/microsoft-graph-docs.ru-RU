---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570941"
---
# <a name="networklocationdetail-resource-type"></a>Тип ресурса networkLocationDetail
Указывает сведения, связанные с сетевую папку. .



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|networkType| Строка перечисления |Предоставляет тип сети. Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.|
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
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
