---
title: Тип ресурса Аудитактивитинитиатор
description: Определяет объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 946f548efc8bb8eea731480f303d8d15703dc018
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033084"
---
# <a name="auditactivityinitiator-resource-type"></a>Тип ресурса Аудитактивитинитиатор

Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (которое считается приложением).

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|программы|[Аппидентити](appidentity.md)|Если ресурс, инициирующий действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, СервицепринЦипалид и Name.|
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
