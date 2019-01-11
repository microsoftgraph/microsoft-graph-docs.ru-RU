---
title: Тип ресурса auditActivityInitiator
description: Идентификатор объекта ресурса, запускает действие. Инициатор может быть пользователем, приложения или системы (который считается, что приложение)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884611"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса auditActivityInitiator
Идентификатор объекта ресурса, запускает действие. Инициатор может быть пользователем, приложения или системы (который считается, что приложение)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|приложение|[appIdentity](appidentity.md)|Если ресурсов, инициализация действие представляет собой приложение, это свойство показывает все приложения связанные сведения, например, appId, имя, servicePrincipalId, имя.|
|user|[удостоверению пользователя](useridentity.md)|Если ресурсов, инициализация действия пользователя, это свойство показывает все пользовательские связанные сведения, например, идентификатор пользователя, имя, UserPrinicpalName.|

## <a name="json-representation"></a>Представление JSON

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
