---
title: Сложный тип approvalStage
description: В управлении правами используется для свойства approvalStages параметров утверждения в свойстве requestApprovalSettings политики назначения пакетов доступа. Указывает основных, резервных и утверждающих эскалацию на каждом этапе. В PIM определяет параметры этапов утверждения в объекте unifiedRoleManagementPolicyApprovalRule.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cfaf9c314002e5fcc0dd2865216ea4346272e4b3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900067"
---
# <a name="approvalstage-complex-type"></a>Сложный тип approvalStage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами используется для свойства **approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики [назначения пакетов доступа](accesspackageassignmentpolicy.md). Указывает основных, резервных и утверждающих эскалацию на каждом этапе.

В PIM определяет параметры этапов утверждения в [объекте unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) . Указывает основных утверждающих лиц и утверждающих эскалацию на каждом этапе, а также необходимость утверждения и эскалации.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | Количество дней, в течение которых запрос может быть ожидающим ответа, прежде чем он будет автоматически отклонен. |
| isApproverJustificationRequired |Boolean | Указывает, требуется ли утверждающему предоставить обоснование для утверждения запроса. |
| isEscalationEnabled |Boolean | Если значение равно true, то на этом этапе утверждения настраивается один или несколько утверждающих эскалацию. |
| escalationTimeInMinutes |Int32 | Если требуется эскалация, время ожидания запроса от основного утверждающего. |
| primaryApprovers | [Коллекция userSet](userset.md)| Пользователи, которым будет предложено утвердить запросы. Коллекция [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) и [externalSponsors](externalsponsors.md). При создании или обновлении [политики](accesspackageassignmentpolicy.md) включите по крайней мере один **userSet** в эту коллекцию. |
| escalationApprovers | [Коллекция userSet](userset.md)| Если эскалация включена, а основные утверждающие не отвечают до укрупнения, пользователи escalationApprovers будут запрашивать утверждение запросов. Это может быть коллекция [объектов singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) и [externalSponsors](externalsponsors.md).  При создании или обновлении [политики, если](accesspackageassignmentpolicy.md) отсутствуют утверждающие эскалации или утверждающие эскалации не требуются для этапа, значение этого свойства должно быть пустой коллекцией.|



## <a name="json-representation"></a>Представление JSON

Ниже приведено представление этапа утверждения запроса в формате JSON.

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


