---
title: сложный тип Аппровалстаже
description: Используется для свойства Аппровалстажес параметров утверждения в свойстве Рекуестаппровалсеттингс политики назначения пакетов Access. Указывает основных, резервных и эскалациых утверждающих каждого этапа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a478f7b0ed06a247ece20ac14763f7de8ff498d
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331430"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="f0f3a-104">сложный тип Аппровалстаже</span><span class="sxs-lookup"><span data-stu-id="f0f3a-104">approvalStage complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f3a-105">Используется для свойства **аппровалстажес** параметров утверждения в свойстве **рекуестаппровалсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0f3a-105">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f0f3a-106">Указывает основных, резервных и эскалациых утверждающих каждого этапа.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-106">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="f0f3a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0f3a-107">Properties</span></span>

| <span data-ttu-id="f0f3a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0f3a-108">Property</span></span>                     | <span data-ttu-id="f0f3a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0f3a-109">Type</span></span>                      | <span data-ttu-id="f0f3a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0f3a-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f0f3a-111">аппровалстажетимеаутиндайс</span><span class="sxs-lookup"><span data-stu-id="f0f3a-111">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="f0f3a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f3a-112">Int32</span></span> | <span data-ttu-id="f0f3a-113">Количество дней, в течение которых запрос может находиться в состоянии ожидания ответа, прежде чем он будет автоматически отклонен.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-113">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="f0f3a-114">исаппровержустификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="f0f3a-114">isApproverJustificationRequired</span></span> |<span data-ttu-id="f0f3a-115">Логический</span><span class="sxs-lookup"><span data-stu-id="f0f3a-115">Boolean</span></span> | <span data-ttu-id="f0f3a-116">Указывает, является ли утверждающий обязательным для предоставления обоснования для утверждения запроса.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-116">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="f0f3a-117">исескалатионенаблед</span><span class="sxs-lookup"><span data-stu-id="f0f3a-117">isEscalationEnabled</span></span> |<span data-ttu-id="f0f3a-118">Логический</span><span class="sxs-lookup"><span data-stu-id="f0f3a-118">Boolean</span></span> | <span data-ttu-id="f0f3a-119">Если задано значение true, на этом этапе утверждения настраивается один или несколько утверждающих.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-119">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="f0f3a-120">ескалатионтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="f0f3a-120">escalationTimeInMinutes</span></span> |<span data-ttu-id="f0f3a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f3a-121">Int32</span></span> | <span data-ttu-id="f0f3a-122">Если требуется эскалация, время, в течение которого запрос может отреагировать от основного утверждающего лица.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-122">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="f0f3a-123">примаряппроверс</span><span class="sxs-lookup"><span data-stu-id="f0f3a-123">primaryApprovers</span></span> | <span data-ttu-id="f0f3a-124">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="f0f3a-124">[userSet](userset.md) collection</span></span>| <span data-ttu-id="f0f3a-125">Пользователи, которые будут запрашивать разрешение на утверждение запросов.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-125">The users who will be asked to approve requests.</span></span> <span data-ttu-id="f0f3a-126">Коллекция объектов [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="f0f3a-126">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="f0f3a-127">ескалатионаппроверс</span><span class="sxs-lookup"><span data-stu-id="f0f3a-127">escalationApprovers</span></span> | <span data-ttu-id="f0f3a-128">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="f0f3a-128">[userSet](userset.md) collection</span></span>| <span data-ttu-id="f0f3a-129">Если распространение включено и основные утверждающие не отвечают на время эскалации, Ескалатионаппроверс — это пользователи, которым будет предложено утвердить запросы.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-129">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="f0f3a-130">Это может быть коллекция [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="f0f3a-130">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="f0f3a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0f3a-131">JSON representation</span></span>

<span data-ttu-id="f0f3a-132">Ниже представлено представление объекта стадии утверждения запроса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0f3a-132">The following is a JSON representation of the request approval stage.</span></span>

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
