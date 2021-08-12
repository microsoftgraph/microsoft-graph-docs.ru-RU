---
title: Тип ресурса auditActivityInitiator
description: Определяет объект ресурса, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением).
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 104e4a05e0c788c9fd71764f815b9305a8554f83d620cc6d01759fc86c794d1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197109"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса auditActivityInitiator

Пространство имен: microsoft.graph

Identity the resource object that initiates the activity. Инициатором может быть пользователь, приложение или система (которая считается приложением).

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|приложение|[appIdentity](appidentity.md)|Если ресурс, инициируя действие, является приложением, это свойство указывает всю связанную с приложением информацию, например appId, Name, servicePrincipalId, Name.|
|пользователь|[userIdentity](useridentity.md)|Если ресурс, инициирующее действие, является пользователем, это свойство указывает всю связанную с пользователем информацию, например userId, Name, UserPrinicpalName.|

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

