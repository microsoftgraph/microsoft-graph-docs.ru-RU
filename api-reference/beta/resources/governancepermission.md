---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3efdebea07bb824b2314af516810ca36ad43adc9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497624"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса Говернанцепермиссион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.|
|isActive|Логический|Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.|
|Действительный|Логический|Указывает, имеет ли запрашивающее назначение роли для уровня доступа.|

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
