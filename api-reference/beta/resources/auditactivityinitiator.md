---
title: Тип ресурса auditActivityInitiator
description: Identity the resource object that initiates the activity. Инициатором может быть пользователь, приложение или система (которая считается приложением)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d131f58057bb3846b2059fa117891dbc405c781223053d80e495fbca788a9688
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206958"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса auditActivityInitiator

Пространство имен: microsoft.graph Identity — ресурсный объект, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|приложение|[appIdentity](appidentity.md)|Если ресурс, инициируя действие, является приложением, это свойство указывает всю связанную с приложением информацию, например appId, Name, servicePrincipalId, Name.|
|user|[userIdentity](useridentity.md)|Если ресурс, инициирующее действие, является пользователем, это свойство указывает всю связанную с пользователем информацию, например userId, Name, UserPrinicpalName.|

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


