---
title: Тип ресурса auditActivityInitiator
description: Identity the resource object that initiates the activity. Инициатором может быть пользователь, приложение или система (которая считается приложением)
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: e681f56f3caf0792241a92ce5137ac8468b623d8
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647164"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса auditActivityInitiator

Пространство имен: microsoft.graph Identity — ресурсный объект, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|приложение|[appIdentity](appidentity.md)|Если инициатором действия является приложение, это свойство указывает все его идентификационные данные, включая appId, displayName, servicePrincipalId и servicePrincipalName.|
|пользователь|[auditUserIdentity](auditUserIdentity.md)|Если инициатором действия является пользователь, это свойство указывает его идентификационные данные, включая их id, displayName и userPrincipalName.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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


