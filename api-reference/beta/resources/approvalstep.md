---
title: тип ресурса approvalStep
description: Объект approvalStep, связанный с accessPackageAssignmentRequest или userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c37320d17a72e0734d856c24cdff49308c9463
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945713"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="e89d8-103">тип ресурса approvalStep</span><span class="sxs-lookup"><span data-stu-id="e89d8-103">approvalStep resource type</span></span>

<span data-ttu-id="e89d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e89d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e89d8-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект approvalStep для решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="e89d8-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="e89d8-106">Он используется для различия решений для различных действий рабочего процесса утверждения, на которые могут действовать одобрители.</span><span class="sxs-lookup"><span data-stu-id="e89d8-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

<span data-ttu-id="e89d8-107">В [userConsentRequests](../resources/userconsentrequest.md)решения об утверждении, связанные с запросом.</span><span class="sxs-lookup"><span data-stu-id="e89d8-107">In [userConsentRequests](../resources/userconsentrequest.md), the approval  decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="e89d8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e89d8-108">Methods</span></span>

| <span data-ttu-id="e89d8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e89d8-109">Method</span></span>       | <span data-ttu-id="e89d8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e89d8-110">Return Type</span></span> | <span data-ttu-id="e89d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e89d8-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="e89d8-112">Утверждение спискаSteps</span><span class="sxs-lookup"><span data-stu-id="e89d8-112">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="e89d8-113">[коллекция approvalStep](approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="e89d8-113">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="e89d8-114">Список объектов **approvalStep,** связанных с объектом **утверждения.**</span><span class="sxs-lookup"><span data-stu-id="e89d8-114">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="e89d8-115">Получить утверждениеStep</span><span class="sxs-lookup"><span data-stu-id="e89d8-115">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="e89d8-116">approvalStep</span><span class="sxs-lookup"><span data-stu-id="e89d8-116">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="e89d8-117">Извлечение свойств объекта **approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="e89d8-117">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="e89d8-118">Обновление approvalStep</span><span class="sxs-lookup"><span data-stu-id="e89d8-118">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="e89d8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e89d8-119">None</span></span> | <span data-ttu-id="e89d8-120">Применить утверждение или отказ в принятии решения по **объекту approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="e89d8-120">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e89d8-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="e89d8-121">Properties</span></span>
|<span data-ttu-id="e89d8-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89d8-122">Property</span></span>|<span data-ttu-id="e89d8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e89d8-123">Type</span></span>|<span data-ttu-id="e89d8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e89d8-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e89d8-125">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="e89d8-125">assignedToMe</span></span>|<span data-ttu-id="e89d8-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e89d8-126">Boolean</span></span>|<span data-ttu-id="e89d8-127">Указывает, назначен ли шаг пользователю вызова для проверки.</span><span class="sxs-lookup"><span data-stu-id="e89d8-127">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="e89d8-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-128">Read-only.</span></span>|
|<span data-ttu-id="e89d8-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e89d8-129">displayName</span></span>|<span data-ttu-id="e89d8-130">Строка</span><span class="sxs-lookup"><span data-stu-id="e89d8-130">String</span></span>|<span data-ttu-id="e89d8-131">Метка, предоставленная создателем политики для определения шага утверждения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-131">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="e89d8-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-132">Read-only.</span></span>|
|<span data-ttu-id="e89d8-133">id</span><span class="sxs-lookup"><span data-stu-id="e89d8-133">id</span></span>|<span data-ttu-id="e89d8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e89d8-134">String</span></span>|<span data-ttu-id="e89d8-135">Идентификатор шага, связанного с объектом утверждения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-135">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="e89d8-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-136">Read-only.</span></span>|
|<span data-ttu-id="e89d8-137">обоснование</span><span class="sxs-lookup"><span data-stu-id="e89d8-137">justification</span></span>|<span data-ttu-id="e89d8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="e89d8-138">String</span></span>|<span data-ttu-id="e89d8-139">Обоснование, связанное с решением о шаге утверждения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-139">The justification associated with the approval step decision.</span></span>|
|<span data-ttu-id="e89d8-140">reviewResult</span><span class="sxs-lookup"><span data-stu-id="e89d8-140">reviewResult</span></span>|<span data-ttu-id="e89d8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="e89d8-141">String</span></span>|<span data-ttu-id="e89d8-142">Результат этой записи утверждения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-142">The result of this approval record.</span></span> <span data-ttu-id="e89d8-143">Возможные значения: `NotReviewed` , `Approved` , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="e89d8-143">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="e89d8-144">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="e89d8-144">reviewedBy</span></span>|<span data-ttu-id="e89d8-145">[коллекция userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="e89d8-145">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="e89d8-146">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="e89d8-146">The identifier of the reviewer.</span></span> <span data-ttu-id="e89d8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-147">Read-only.</span></span>|
|<span data-ttu-id="e89d8-148">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="e89d8-148">reviewedDateTime</span></span>|<span data-ttu-id="e89d8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e89d8-149">DateTimeOffset</span></span>|<span data-ttu-id="e89d8-150">Дата и время записи решения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-150">The date and time when a decision was recorded.</span></span> <span data-ttu-id="e89d8-151">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e89d8-151">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e89d8-152">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e89d8-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e89d8-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-153">Read-only.</span></span>|
|<span data-ttu-id="e89d8-154">status</span><span class="sxs-lookup"><span data-stu-id="e89d8-154">status</span></span>|<span data-ttu-id="e89d8-155">String</span><span class="sxs-lookup"><span data-stu-id="e89d8-155">String</span></span>|<span data-ttu-id="e89d8-156">Состояние шага.</span><span class="sxs-lookup"><span data-stu-id="e89d8-156">The step status.</span></span> <span data-ttu-id="e89d8-157">Возможные значения: `InProgress` `Initializing` , , `Completed` `Expired` .</span><span class="sxs-lookup"><span data-stu-id="e89d8-157">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="e89d8-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e89d8-158">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e89d8-159">Связи</span><span class="sxs-lookup"><span data-stu-id="e89d8-159">Relationships</span></span>
|<span data-ttu-id="e89d8-160">Связь</span><span class="sxs-lookup"><span data-stu-id="e89d8-160">Relationship</span></span>|<span data-ttu-id="e89d8-161">Тип</span><span class="sxs-lookup"><span data-stu-id="e89d8-161">Type</span></span>|<span data-ttu-id="e89d8-162">Описание</span><span class="sxs-lookup"><span data-stu-id="e89d8-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e89d8-163">утверждение</span><span class="sxs-lookup"><span data-stu-id="e89d8-163">approval</span></span>|<span data-ttu-id="e89d8-164">[коллекция утверждений](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="e89d8-164">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="e89d8-165">Объект утверждения решений, связанных с `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="e89d8-165">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e89d8-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e89d8-166">JSON representation</span></span>
<span data-ttu-id="e89d8-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e89d8-167">The following is a JSON representation of the resource.</span></span>
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
