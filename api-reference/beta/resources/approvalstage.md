---
title: сложный тип Аппровалстаже
description: Используется для свойства Аппровалстажес параметров утверждения в свойстве Рекуестаппровалсеттингс политики назначения пакетов Access. Указывает основных, резервных и эскалациых утверждающих каждого этапа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0edcb4af5ae6bbc154d0748b57ec83efcb3137f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508228"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="5c33e-104">сложный тип Аппровалстаже</span><span class="sxs-lookup"><span data-stu-id="5c33e-104">approvalStage complex type</span></span>

<span data-ttu-id="5c33e-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c33e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c33e-106">Используется для свойства **аппровалстажес** параметров утверждения в свойстве **рекуестаппровалсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c33e-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="5c33e-107">Указывает основных, резервных и эскалациых утверждающих каждого этапа.</span><span class="sxs-lookup"><span data-stu-id="5c33e-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="5c33e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c33e-108">Properties</span></span>

| <span data-ttu-id="5c33e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c33e-109">Property</span></span>                     | <span data-ttu-id="5c33e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5c33e-110">Type</span></span>                      | <span data-ttu-id="5c33e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c33e-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="5c33e-112">аппровалстажетимеаутиндайс</span><span class="sxs-lookup"><span data-stu-id="5c33e-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="5c33e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5c33e-113">Int32</span></span> | <span data-ttu-id="5c33e-114">Количество дней, в течение которых запрос может находиться в состоянии ожидания ответа, прежде чем он будет автоматически отклонен.</span><span class="sxs-lookup"><span data-stu-id="5c33e-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="5c33e-115">исаппровержустификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="5c33e-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="5c33e-116">Логический</span><span class="sxs-lookup"><span data-stu-id="5c33e-116">Boolean</span></span> | <span data-ttu-id="5c33e-117">Указывает, является ли утверждающий обязательным для предоставления обоснования для утверждения запроса.</span><span class="sxs-lookup"><span data-stu-id="5c33e-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="5c33e-118">исескалатионенаблед</span><span class="sxs-lookup"><span data-stu-id="5c33e-118">isEscalationEnabled</span></span> |<span data-ttu-id="5c33e-119">Логический</span><span class="sxs-lookup"><span data-stu-id="5c33e-119">Boolean</span></span> | <span data-ttu-id="5c33e-120">Если задано значение true, на этом этапе утверждения настраивается один или несколько утверждающих.</span><span class="sxs-lookup"><span data-stu-id="5c33e-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="5c33e-121">ескалатионтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="5c33e-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="5c33e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5c33e-122">Int32</span></span> | <span data-ttu-id="5c33e-123">Если требуется эскалация, время, в течение которого запрос может отреагировать от основного утверждающего лица.</span><span class="sxs-lookup"><span data-stu-id="5c33e-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="5c33e-124">примаряппроверс</span><span class="sxs-lookup"><span data-stu-id="5c33e-124">primaryApprovers</span></span> | <span data-ttu-id="5c33e-125">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="5c33e-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="5c33e-126">Пользователи, которые будут запрашивать разрешение на утверждение запросов.</span><span class="sxs-lookup"><span data-stu-id="5c33e-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="5c33e-127">Коллекция объектов [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="5c33e-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="5c33e-128">ескалатионаппроверс</span><span class="sxs-lookup"><span data-stu-id="5c33e-128">escalationApprovers</span></span> | <span data-ttu-id="5c33e-129">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="5c33e-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="5c33e-130">Если распространение включено и основные утверждающие не отвечают на время эскалации, Ескалатионаппроверс — это пользователи, которым будет предложено утвердить запросы.</span><span class="sxs-lookup"><span data-stu-id="5c33e-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="5c33e-131">Это может быть коллекция [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="5c33e-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="5c33e-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c33e-132">JSON representation</span></span>

<span data-ttu-id="5c33e-133">Ниже представлено представление объекта стадии утверждения запроса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c33e-133">The following is a JSON representation of the request approval stage.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage",
  "baseType": ""
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
