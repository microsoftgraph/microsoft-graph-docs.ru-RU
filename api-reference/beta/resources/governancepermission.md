---
title: тип ресурса governancePermission
description: 'Представляет разрешение доступа, которое у governanceSubject имеется для определенного governanceResource.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 0cb80e78e3cbdb2c019347d28ff79be262ec7b99
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696219"
---
# <a name="governancepermission-resource-type"></a>тип ресурса governancePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1resourceroles-deprecation.md)]

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


