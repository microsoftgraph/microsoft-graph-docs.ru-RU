---
title: Тип ресурса governancePermission
description: 'Представляет разрешение на доступ, которое имеется у governanceSubject к определенному governanceResource.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128847"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса governancePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет разрешение на доступ, которое [имеется у governanceSubject](../resources/governancesubject.md) к определенному [governanceResource.](../resources/governanceresource.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|Строка|Уровень доступа. Допустимые значения: ``None`` , , , и ``UserRead`` ``AdminRead`` ``AdminReadWrite`` .|
|isActive|Boolean|Указать, есть ли у запрашивателя назначение активной роли для уровня доступа.|
|isEligible|Boolean|Указать, есть ли у запрашивателя право на назначение роли для уровня доступа.|

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


