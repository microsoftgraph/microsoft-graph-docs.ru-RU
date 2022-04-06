---
title: тип ресурса governancePermission
description: 'Представляет разрешение доступа, которое у governanceSubject имеется для определенного governanceResource.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: b4244335bba57c9ff5200099520e2e0b2a5e98c2
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510410"
---
# <a name="governancepermission-resource-type"></a>тип ресурса governancePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет разрешение доступа, которое [у governanceSubject](../resources/governancesubject.md) имеется для определенного [governanceResource](../resources/governanceresource.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|Строка|Уровень доступа. Допустимые значения: ``None``, ``UserRead``, ``AdminRead``и ``AdminReadWrite``.|
|isActive|Boolean|Указать, есть ли у запрашивателя какие-либо активные назначения ролей для уровня доступа.|
|isEligible|Boolean|Указать, имеется ли у запросителя любое назначение ролей для уровня доступа.|

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


