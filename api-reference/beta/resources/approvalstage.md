---
title: Сложный тип approvalStage
description: Используется для свойства approvalStages параметров утверждения в свойстве requestApprovalSettings политики назначения пакета доступа. Указывает основных, откатных и утвердителей эскалации каждого этапа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d24f8def3520cf2605f30dc47ab06f52e09fc163
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135261"
---
# <a name="approvalstage-complex-type"></a>Сложный тип approvalStage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** [политики назначения пакета доступа.](accesspackageassignmentpolicy.md) Указывает основных, откатных и утвердителей эскалации каждого этапа.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | Количество дней, в течение которые запрос может быть ожидающих ответа, прежде чем он будет автоматически отклонен. |
| isApproverJustificationRequired |Boolean | Указывает, требуется ли утвердитель предоставить обоснование для утверждения запроса. |
| isEscalationEnabled |Boolean | Если установлено true, на этом этапе утверждения настраивается один или несколько утвержденных разрешений эскалации. |
| escalationTimeInMinutes |Int32 | Если требуется эскалация, время ожидания ответа от основного утвержденного запроса. |
| primaryApprovers | [Коллекция userSet](userset.md)| Пользователи, которым будет предложено утвердить запросы. Коллекция [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md) и [externalSponsors.](externalsponsors.md) |
| escalationApprovers | [Коллекция userSet](userset.md)| Если эскалация включена, а основные утвержденные не отвечают до эскалации, пользователи, которым будет предложено утвердить запросы, будут запрашивать. Это может быть коллекция [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md) и [externalSponsors.](externalsponsors.md)|



## <a name="json-representation"></a>Представление в формате JSON

Ниже приводится представление этапа утверждения запроса в JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage"
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


