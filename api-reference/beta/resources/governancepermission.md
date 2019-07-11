---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
ms.openlocfilehash: cd5b15a85dee7a193962a6072bcdf34b1d4f131a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621307"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса Говернанцепермиссион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.|
|isActive|Boolean|Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.|
|Действительный|Boolean|Указывает, имеет ли запрашивающее назначение роли для уровня доступа.|

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
