---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 14c8335cab401c246f95452dac699daa4f81ea93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033848"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса Говернанцепермиссион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения: ``None`` ,, ``UserRead`` ``AdminRead`` и ``AdminReadWrite`` .|
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


