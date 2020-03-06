---
title: Тип ресурса Аудитактивитинитиатор
description: Определяет объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ed2a68d3e3fa07edb5b5b2ce0d969287ba9a7a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532051"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса Аудитактивитинитиатор

Пространство имен: microsoft.graph

Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (которое считается приложением).

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
