---
title: тип approvalStage сложный
description: Используется для свойства approvalStages параметров утверждения в свойстве requestApprovalSettings политики назначения пакета доступа. Указывает основные, откаты и утверждения эскалации на каждом этапе.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd5a27a66d335dfe56acfbb0d30771ddbd9a703c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336384"
---
# <a name="approvalstage-complex-type"></a>тип approvalStage сложный

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа](accesspackageassignmentpolicy.md). Указывает основные, откаты и утверждения эскалации на каждом этапе.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | Количество дней, в которые запрос может быть отложен до автоматического отключаемого ответа. |
| isApproverJustificationRequired |Boolean | Указывает, требуется ли одобрение для обоснования утверждения запроса. |
| isEscalationEnabled |Boolean | Если это так, то на этом этапе утверждения настраивается один или несколько утверждений эскалации. |
| escalationTimeInMinutes |Int32 | Если требуется эскалация, время ожидания запроса от основного утвержденного. |
| primaryApprovers | [коллекция userSet](userset.md)| Пользователи, которым будет предложено утвердить запросы. Коллекция [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) и [externalSponsors](externalsponsors.md). При создании или обновлении [политики](accesspackageassignmentpolicy.md) включаем по крайней мере одного **пользователяSet** в эту коллекцию. |
| escalationApprovers | [коллекция userSet](userset.md)| Если эскалация включена, а основные одобрители не реагируют до времени эскалации, пользователи, которым будет предложено утвердить запросы, будут запрашивать. Это может быть коллекция [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) и [externalSponsors](externalsponsors.md).  При создании или обновлении [политики, если](accesspackageassignmentpolicy.md) для стадии не требуются утверждения эскалации или не требуются утверждения эскалации, значение этого свойства должно быть пустой коллекцией.|



## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON стадии утверждения запроса.

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


