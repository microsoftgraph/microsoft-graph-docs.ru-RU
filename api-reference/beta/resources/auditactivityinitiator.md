---
title: Тип ресурса auditActivityInitiator
description: Удостоверение объекта ресурса, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: 71aa5e2bd09d66a2aea49058ceffea3e017eaf4d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131637"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса auditActivityInitiator

Пространство имен: удостоверение microsoft.graph для объекта ресурса, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|приложение|[appIdentity](appidentity.md)|Если ресурс, инициируя действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, servicePrincipalId, Name.|
|user|[userIdentity](useridentity.md)|Если ресурсом, инициирующим действие, является пользователь, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, UserPrinicpalName.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


