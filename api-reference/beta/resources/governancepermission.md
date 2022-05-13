---
title: Тип ресурса governancePermission
description: 'Представляет разрешение доступа, которое объект governanceSubject имеет к определенному объекту governanceResource.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: b88900882ecceabcfe5101aa4564b88116df605f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397966"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса governancePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет разрешение доступа, которое [объект governanceSubject](../resources/governancesubject.md) имеет к определенному [объекту governanceResource](../resources/governanceresource.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения: ``None``, ``UserRead``, и ``AdminReadWrite````AdminRead``.|
|isActive|Логическое|Укажите, имеет ли инициатор запроса активное назначение ролей для уровня доступа.|
|isEligible|Логическое|Укажите, имеет ли инициатор запроса любое допустимое назначение роли для уровня доступа.|

## <a name="json-representation"></a>Представление в формате JSON

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


