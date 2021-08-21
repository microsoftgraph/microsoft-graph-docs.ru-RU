---
title: тип ресурса governancePermission
description: 'Представляет разрешение доступа, которое у governanceSubject имеется для определенного governanceResource.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: c094050f32b020c204d645dfc0c398ad5bfa5d20
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453732"
---
# <a name="governancepermission-resource-type"></a>тип ресурса governancePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет разрешение доступа, которое [у governanceSubject](../resources/governancesubject.md) имеется для определенного [governanceResource.](../resources/governanceresource.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения: ``None`` ``UserRead`` , , и ``AdminRead`` ``AdminReadWrite`` .|
|isActive|Логический|Указать, есть ли у запрашивателя какие-либо активные назначения ролей для уровня доступа.|
|isEligible|Логический|Указать, имеется ли у запросителя любое назначение ролей для уровня доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```


