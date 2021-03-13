---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с accessPackageAssignmentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d46630b563674153ef687a8e8f86dce70eec9985
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761263"
---
# <a name="approval-resource-type"></a><span data-ttu-id="346d9-103">Тип ресурса утверждения</span><span class="sxs-lookup"><span data-stu-id="346d9-103">approval resource type</span></span>

<span data-ttu-id="346d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="346d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="346d9-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект утверждения решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="346d9-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="346d9-106">Запрос на один шаг может иметь один шаг, связанный с ним, на который могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="346d9-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="346d9-107">Кроме того, многоэтапный запрос может иметь несколько действий, связанных с ним, на которые могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="346d9-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="346d9-108">Однако в многоэтапных утверждениях показаны как ожидающих, так и ранее завершенных действий.</span><span class="sxs-lookup"><span data-stu-id="346d9-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

## <a name="methods"></a><span data-ttu-id="346d9-109">Методы</span><span class="sxs-lookup"><span data-stu-id="346d9-109">Methods</span></span>

| <span data-ttu-id="346d9-110">Метод</span><span class="sxs-lookup"><span data-stu-id="346d9-110">Method</span></span>       | <span data-ttu-id="346d9-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="346d9-111">Return Type</span></span> | <span data-ttu-id="346d9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="346d9-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="346d9-113">Получить утверждение</span><span class="sxs-lookup"><span data-stu-id="346d9-113">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="346d9-114">утверждение</span><span class="sxs-lookup"><span data-stu-id="346d9-114">approval</span></span>](approval.md) | <span data-ttu-id="346d9-115">Извлечение свойств объекта **утверждения.**</span><span class="sxs-lookup"><span data-stu-id="346d9-115">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="346d9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="346d9-116">Properties</span></span>
|<span data-ttu-id="346d9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="346d9-117">Property</span></span>|<span data-ttu-id="346d9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="346d9-118">Type</span></span>|<span data-ttu-id="346d9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="346d9-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346d9-120">id</span><span class="sxs-lookup"><span data-stu-id="346d9-120">id</span></span>|<span data-ttu-id="346d9-121">String</span><span class="sxs-lookup"><span data-stu-id="346d9-121">String</span></span>|<span data-ttu-id="346d9-122">Идентификатор объекта утверждения.</span><span class="sxs-lookup"><span data-stu-id="346d9-122">The identifier of the approval object.</span></span>|
|<span data-ttu-id="346d9-123">действия</span><span class="sxs-lookup"><span data-stu-id="346d9-123">steps</span></span>|<span data-ttu-id="346d9-124">[коллекция approvalStep](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="346d9-124">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="346d9-125">Используется для представления решения, связанного с одним шагом в процессе утверждения, настроенного в [approvalStage.](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="346d9-125">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="346d9-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="346d9-126">Relationships</span></span>
|<span data-ttu-id="346d9-127">Связь</span><span class="sxs-lookup"><span data-stu-id="346d9-127">Relationship</span></span>|<span data-ttu-id="346d9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="346d9-128">Type</span></span>|<span data-ttu-id="346d9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="346d9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346d9-130">stages</span><span class="sxs-lookup"><span data-stu-id="346d9-130">stages</span></span>|<span data-ttu-id="346d9-131">[коллекция approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="346d9-131">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="346d9-132">Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="346d9-132">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="346d9-133">Указывает основные, откаты и утверждения эскалации на каждом этапе.</span><span class="sxs-lookup"><span data-stu-id="346d9-133">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="346d9-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="346d9-134">JSON representation</span></span>
<span data-ttu-id="346d9-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="346d9-135">The following is a JSON representation of the resource.</span></span>
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
