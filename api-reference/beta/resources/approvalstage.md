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
# <a name="approvalstage-complex-type"></a><span data-ttu-id="47e81-104">Сложный тип approvalStage</span><span class="sxs-lookup"><span data-stu-id="47e81-104">approvalStage complex type</span></span>

<span data-ttu-id="47e81-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e81-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e81-106">Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** [политики назначения пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="47e81-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="47e81-107">Указывает основных, откатных и утвердителей эскалации каждого этапа.</span><span class="sxs-lookup"><span data-stu-id="47e81-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="47e81-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47e81-108">Properties</span></span>

| <span data-ttu-id="47e81-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47e81-109">Property</span></span>                     | <span data-ttu-id="47e81-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47e81-110">Type</span></span>                      | <span data-ttu-id="47e81-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47e81-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="47e81-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="47e81-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="47e81-113">Int32</span><span class="sxs-lookup"><span data-stu-id="47e81-113">Int32</span></span> | <span data-ttu-id="47e81-114">Количество дней, в течение которые запрос может быть ожидающих ответа, прежде чем он будет автоматически отклонен.</span><span class="sxs-lookup"><span data-stu-id="47e81-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="47e81-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="47e81-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="47e81-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e81-116">Boolean</span></span> | <span data-ttu-id="47e81-117">Указывает, требуется ли утвердитель предоставить обоснование для утверждения запроса.</span><span class="sxs-lookup"><span data-stu-id="47e81-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="47e81-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="47e81-118">isEscalationEnabled</span></span> |<span data-ttu-id="47e81-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e81-119">Boolean</span></span> | <span data-ttu-id="47e81-120">Если установлено true, на этом этапе утверждения настраивается один или несколько утвержденных разрешений эскалации.</span><span class="sxs-lookup"><span data-stu-id="47e81-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="47e81-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="47e81-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="47e81-122">Int32</span><span class="sxs-lookup"><span data-stu-id="47e81-122">Int32</span></span> | <span data-ttu-id="47e81-123">Если требуется эскалация, время ожидания ответа от основного утвержденного запроса.</span><span class="sxs-lookup"><span data-stu-id="47e81-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="47e81-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="47e81-124">primaryApprovers</span></span> | <span data-ttu-id="47e81-125">[Коллекция userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="47e81-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="47e81-126">Пользователи, которым будет предложено утвердить запросы.</span><span class="sxs-lookup"><span data-stu-id="47e81-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="47e81-127">Коллекция [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md) и [externalSponsors.](externalsponsors.md)</span><span class="sxs-lookup"><span data-stu-id="47e81-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="47e81-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="47e81-128">escalationApprovers</span></span> | <span data-ttu-id="47e81-129">[Коллекция userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="47e81-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="47e81-130">Если эскалация включена, а основные утвержденные не отвечают до эскалации, пользователи, которым будет предложено утвердить запросы, будут запрашивать.</span><span class="sxs-lookup"><span data-stu-id="47e81-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="47e81-131">Это может быть коллекция [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md) и [externalSponsors.](externalsponsors.md)</span><span class="sxs-lookup"><span data-stu-id="47e81-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="47e81-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47e81-132">JSON representation</span></span>

<span data-ttu-id="47e81-133">Ниже приводится представление этапа утверждения запроса в JSON.</span><span class="sxs-lookup"><span data-stu-id="47e81-133">The following is a JSON representation of the request approval stage.</span></span>

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


