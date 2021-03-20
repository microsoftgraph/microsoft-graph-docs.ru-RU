---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с accessPackageAssignmentRequest или userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f6751807f0dcb042958104c4b3146a555b22189
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945729"
---
# <a name="approval-resource-type"></a><span data-ttu-id="c0e0e-103">Тип ресурса утверждения</span><span class="sxs-lookup"><span data-stu-id="c0e0e-103">approval resource type</span></span>

<span data-ttu-id="c0e0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0e0e-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект утверждения решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="c0e0e-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="c0e0e-106">Запрос на один шаг может иметь один шаг, связанный с ним, на который могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="c0e0e-107">Кроме того, многоэтапный запрос может иметь несколько действий, связанных с ним, на которые могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="c0e0e-108">Однако в многоэтапных утверждениях показаны как ожидающих, так и ранее завершенных действий.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

<span data-ttu-id="c0e0e-109">В [userConsentRequests](../resources/userconsentrequest.md)объект утверждения решений, связанных с запросом.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-109">In [userConsentRequests](../resources/userconsentrequest.md), the approval object for decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="c0e0e-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c0e0e-110">Methods</span></span>

| <span data-ttu-id="c0e0e-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c0e0e-111">Method</span></span>       | <span data-ttu-id="c0e0e-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0e0e-112">Return Type</span></span> | <span data-ttu-id="c0e0e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e0e-113">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="c0e0e-114">Получить утверждение</span><span class="sxs-lookup"><span data-stu-id="c0e0e-114">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="c0e0e-115">утверждение</span><span class="sxs-lookup"><span data-stu-id="c0e0e-115">approval</span></span>](approval.md) | <span data-ttu-id="c0e0e-116">Извлечение свойств объекта **утверждения.**</span><span class="sxs-lookup"><span data-stu-id="c0e0e-116">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="c0e0e-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0e0e-117">Properties</span></span>
|<span data-ttu-id="c0e0e-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0e0e-118">Property</span></span>|<span data-ttu-id="c0e0e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e0e-119">Type</span></span>|<span data-ttu-id="c0e0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e0e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e0e-121">id</span><span class="sxs-lookup"><span data-stu-id="c0e0e-121">id</span></span>|<span data-ttu-id="c0e0e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c0e0e-122">String</span></span>|<span data-ttu-id="c0e0e-123">Идентификатор объекта утверждения.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-123">The identifier of the approval object.</span></span>|
|<span data-ttu-id="c0e0e-124">действия</span><span class="sxs-lookup"><span data-stu-id="c0e0e-124">steps</span></span>|<span data-ttu-id="c0e0e-125">[коллекция approvalStep](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="c0e0e-125">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="c0e0e-126">Используется для представления решения, связанного с одним шагом в процессе утверждения, настроенного в [approvalStage.](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="c0e0e-126">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0e0e-127">Связи</span><span class="sxs-lookup"><span data-stu-id="c0e0e-127">Relationships</span></span>
|<span data-ttu-id="c0e0e-128">Связь</span><span class="sxs-lookup"><span data-stu-id="c0e0e-128">Relationship</span></span>|<span data-ttu-id="c0e0e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e0e-129">Type</span></span>|<span data-ttu-id="c0e0e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e0e-131">stages</span><span class="sxs-lookup"><span data-stu-id="c0e0e-131">stages</span></span>|<span data-ttu-id="c0e0e-132">[коллекция approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="c0e0e-132">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="c0e0e-133">Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0e0e-133">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="c0e0e-134">Указывает основные, откаты и утверждения эскалации на каждом этапе.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-134">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c0e0e-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0e0e-135">JSON representation</span></span>
<span data-ttu-id="c0e0e-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0e0e-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
