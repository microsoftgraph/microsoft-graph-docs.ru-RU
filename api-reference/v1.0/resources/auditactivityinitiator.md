---
title: Тип ресурса auditActivityInitiator
description: Определяет объект ресурса, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением).
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fac9b0852a53390b4c9f51ede4fec1acd707d4fe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127068"
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

