---
title: Тип ресурса Аудитактивитинитиатор
description: Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: f5f472be4d8fd40d053efa4ae2b5ad38e4925c76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998916"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса Аудитактивитинитиатор

Пространство имен: Microsoft. Graph Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|программы|[аппидентити](appidentity.md)|Если ресурс, инициирующий действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, СервицепринЦипалид и Name.|
|user|[userIdentity](useridentity.md)|Если ресурс, инициирующий действие, является пользователем, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, Усерприникпалнаме.|

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


