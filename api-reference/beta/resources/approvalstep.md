---
title: тип ресурса approvalStep
description: Объект approvalStep, связанный с accessPackageAssignmentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 263e809e5858cdc23b34b8401171bb5fce668721
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761256"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="184d3-103">тип ресурса approvalStep</span><span class="sxs-lookup"><span data-stu-id="184d3-103">approvalStep resource type</span></span>

<span data-ttu-id="184d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="184d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="184d3-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект approvalStep для решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="184d3-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="184d3-106">Он используется для различия решений для различных действий рабочего процесса утверждения, на которые могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="184d3-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

## <a name="methods"></a><span data-ttu-id="184d3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="184d3-107">Methods</span></span>

| <span data-ttu-id="184d3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="184d3-108">Method</span></span>       | <span data-ttu-id="184d3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="184d3-109">Return Type</span></span> | <span data-ttu-id="184d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="184d3-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="184d3-111">Утверждение спискаSteps</span><span class="sxs-lookup"><span data-stu-id="184d3-111">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="184d3-112">[коллекция approvalStep](approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="184d3-112">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="184d3-113">Список объектов **approvalStep,** связанных с объектом **утверждения.**</span><span class="sxs-lookup"><span data-stu-id="184d3-113">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="184d3-114">Получить утверждениеStep</span><span class="sxs-lookup"><span data-stu-id="184d3-114">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="184d3-115">approvalStep</span><span class="sxs-lookup"><span data-stu-id="184d3-115">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="184d3-116">Извлечение свойств объекта **approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="184d3-116">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="184d3-117">Обновление approvalStep</span><span class="sxs-lookup"><span data-stu-id="184d3-117">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="184d3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="184d3-118">None</span></span> | <span data-ttu-id="184d3-119">Применить утверждение или отказ в принятии решения по **объекту approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="184d3-119">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="184d3-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="184d3-120">Properties</span></span>
|<span data-ttu-id="184d3-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="184d3-121">Property</span></span>|<span data-ttu-id="184d3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="184d3-122">Type</span></span>|<span data-ttu-id="184d3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="184d3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184d3-124">id</span><span class="sxs-lookup"><span data-stu-id="184d3-124">id</span></span>|<span data-ttu-id="184d3-125">String</span><span class="sxs-lookup"><span data-stu-id="184d3-125">String</span></span>|<span data-ttu-id="184d3-126">Идентификатор шага, связанного с объектом утверждения.</span><span class="sxs-lookup"><span data-stu-id="184d3-126">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="184d3-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="184d3-127">Read-only.</span></span>|
|<span data-ttu-id="184d3-128">displayName</span><span class="sxs-lookup"><span data-stu-id="184d3-128">displayName</span></span>|<span data-ttu-id="184d3-129">String</span><span class="sxs-lookup"><span data-stu-id="184d3-129">String</span></span>|<span data-ttu-id="184d3-130">Метка, предоставленная создателем политики для определения шага утверждения.</span><span class="sxs-lookup"><span data-stu-id="184d3-130">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="184d3-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="184d3-131">Read-only</span></span>|
|<span data-ttu-id="184d3-132">status</span><span class="sxs-lookup"><span data-stu-id="184d3-132">status</span></span>|<span data-ttu-id="184d3-133">String</span><span class="sxs-lookup"><span data-stu-id="184d3-133">String</span></span>|<span data-ttu-id="184d3-134">Состояние шага.</span><span class="sxs-lookup"><span data-stu-id="184d3-134">The step status.</span></span> <span data-ttu-id="184d3-135">Возможные значения: `InProgress` или `Completed` .</span><span class="sxs-lookup"><span data-stu-id="184d3-135">Possible values: `InProgress` or `Completed`.</span></span> <span data-ttu-id="184d3-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="184d3-136">Read-only.</span></span>|
|<span data-ttu-id="184d3-137">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="184d3-137">assignedToMe</span></span>|<span data-ttu-id="184d3-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="184d3-138">Boolean</span></span>|<span data-ttu-id="184d3-139">Указывает, назначен ли шаг пользователю вызова для проверки.</span><span class="sxs-lookup"><span data-stu-id="184d3-139">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="184d3-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="184d3-140">Read-only.</span></span>|
|<span data-ttu-id="184d3-141">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="184d3-141">reviewedBy</span></span>|<span data-ttu-id="184d3-142">[коллекция userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="184d3-142">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="184d3-143">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="184d3-143">The identifier of the reviewer.</span></span> <span data-ttu-id="184d3-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="184d3-144">Read-only.</span></span>|
|<span data-ttu-id="184d3-145">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="184d3-145">reviewedDateTime</span></span>|<span data-ttu-id="184d3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="184d3-146">DateTimeOffset</span></span>|<span data-ttu-id="184d3-147">Дата и время записи решения.</span><span class="sxs-lookup"><span data-stu-id="184d3-147">The date and time when a decision was recorded.</span></span> <span data-ttu-id="184d3-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="184d3-148">Read-only.</span></span>|
|<span data-ttu-id="184d3-149">reviewResult</span><span class="sxs-lookup"><span data-stu-id="184d3-149">reviewResult</span></span>|<span data-ttu-id="184d3-150">String</span><span class="sxs-lookup"><span data-stu-id="184d3-150">String</span></span>|<span data-ttu-id="184d3-151">Результат этой записи утверждения.</span><span class="sxs-lookup"><span data-stu-id="184d3-151">The result of this approval record.</span></span> <span data-ttu-id="184d3-152">Возможные значения: `NotReviewed` , `Approved` , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="184d3-152">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="184d3-153">обоснование</span><span class="sxs-lookup"><span data-stu-id="184d3-153">justification</span></span>|<span data-ttu-id="184d3-154">String</span><span class="sxs-lookup"><span data-stu-id="184d3-154">String</span></span>|<span data-ttu-id="184d3-155">Обоснование, связанное с решением о шаге утверждения.</span><span class="sxs-lookup"><span data-stu-id="184d3-155">The justification associated with the approval step decision.</span></span>|

## <a name="relationships"></a><span data-ttu-id="184d3-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="184d3-156">Relationships</span></span>
|<span data-ttu-id="184d3-157">Связь</span><span class="sxs-lookup"><span data-stu-id="184d3-157">Relationship</span></span>|<span data-ttu-id="184d3-158">Тип</span><span class="sxs-lookup"><span data-stu-id="184d3-158">Type</span></span>|<span data-ttu-id="184d3-159">Описание</span><span class="sxs-lookup"><span data-stu-id="184d3-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184d3-160">утверждение</span><span class="sxs-lookup"><span data-stu-id="184d3-160">approval</span></span>|<span data-ttu-id="184d3-161">[коллекция утверждений](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="184d3-161">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="184d3-162">Объект утверждения решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="184d3-162">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="184d3-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="184d3-163">JSON representation</span></span>
<span data-ttu-id="184d3-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="184d3-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalStep",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": true,
  "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String",
}
```
