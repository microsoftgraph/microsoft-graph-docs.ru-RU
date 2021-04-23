---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с accessPackageAssignmentRequest или userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8365ff5f42d85698965fe0d63d70c719a037f530
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961375"
---
# <a name="approval-resource-type"></a><span data-ttu-id="31f9f-103">Тип ресурса утверждения</span><span class="sxs-lookup"><span data-stu-id="31f9f-103">approval resource type</span></span>

<span data-ttu-id="31f9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31f9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31f9f-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект утверждения решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="31f9f-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="31f9f-106">Запрос на один шаг может иметь один шаг, связанный с ним, на который могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="31f9f-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="31f9f-107">Кроме того, многоэтапный запрос может иметь несколько действий, связанных с ним, на которые могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="31f9f-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="31f9f-108">Однако в многоэтапных утверждениях показаны как ожидающих, так и ранее завершенных действий.</span><span class="sxs-lookup"><span data-stu-id="31f9f-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

<span data-ttu-id="31f9f-109">В [userConsentRequests](../resources/userconsentrequest.md)объект утверждения решений, связанных с запросом.</span><span class="sxs-lookup"><span data-stu-id="31f9f-109">In [userConsentRequests](../resources/userconsentrequest.md), the approval object for decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="31f9f-110">Методы</span><span class="sxs-lookup"><span data-stu-id="31f9f-110">Methods</span></span>

| <span data-ttu-id="31f9f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="31f9f-111">Method</span></span>       | <span data-ttu-id="31f9f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31f9f-112">Return Type</span></span> | <span data-ttu-id="31f9f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="31f9f-113">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="31f9f-114">Получить утверждение</span><span class="sxs-lookup"><span data-stu-id="31f9f-114">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="31f9f-115">утверждение</span><span class="sxs-lookup"><span data-stu-id="31f9f-115">approval</span></span>](approval.md) | <span data-ttu-id="31f9f-116">Извлечение свойств объекта **утверждения.**</span><span class="sxs-lookup"><span data-stu-id="31f9f-116">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="31f9f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="31f9f-117">Properties</span></span>
|<span data-ttu-id="31f9f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="31f9f-118">Property</span></span>|<span data-ttu-id="31f9f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="31f9f-119">Type</span></span>|<span data-ttu-id="31f9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="31f9f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31f9f-121">id</span><span class="sxs-lookup"><span data-stu-id="31f9f-121">id</span></span>|<span data-ttu-id="31f9f-122">String</span><span class="sxs-lookup"><span data-stu-id="31f9f-122">String</span></span>|<span data-ttu-id="31f9f-123">Идентификатор объекта утверждения.</span><span class="sxs-lookup"><span data-stu-id="31f9f-123">The identifier of the approval object.</span></span>  <span data-ttu-id="31f9f-124">В управлении правами это тот же идентификатор, что и идентификатор запроса на назначение пакета [доступа.](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="31f9f-124">In entitlement management, it is the same identifier as the identifier of the [access package assignment request](accesspackageassignmentrequest.md).</span></span>|
|<span data-ttu-id="31f9f-125">действия</span><span class="sxs-lookup"><span data-stu-id="31f9f-125">steps</span></span>|<span data-ttu-id="31f9f-126">[коллекция approvalStep](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="31f9f-126">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="31f9f-127">Используется для представления решения, связанного с одним шагом в процессе утверждения, настроенного в [approvalStage.](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="31f9f-127">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="31f9f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="31f9f-128">Relationships</span></span>
|<span data-ttu-id="31f9f-129">Связь</span><span class="sxs-lookup"><span data-stu-id="31f9f-129">Relationship</span></span>|<span data-ttu-id="31f9f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31f9f-130">Type</span></span>|<span data-ttu-id="31f9f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31f9f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31f9f-132">stages</span><span class="sxs-lookup"><span data-stu-id="31f9f-132">stages</span></span>|<span data-ttu-id="31f9f-133">[коллекция approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="31f9f-133">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="31f9f-134">Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="31f9f-134">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="31f9f-135">Указывает основные, откаты и утверждения эскалации на каждом этапе.</span><span class="sxs-lookup"><span data-stu-id="31f9f-135">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="31f9f-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31f9f-136">JSON representation</span></span>
<span data-ttu-id="31f9f-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31f9f-137">The following is a JSON representation of the resource.</span></span>
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
