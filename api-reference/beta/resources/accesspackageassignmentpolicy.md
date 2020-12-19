---
title: Тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа определяет политику, с помощью которой субъекты могут запрашивать или получать доступ к пакету доступа через назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c963030980e96c5baabe8bcfe9103d4dc5167979
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719764"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="8e183-103">Тип ресурса accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="8e183-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e183-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e183-105">В управлении правами [Azure AD](entitlementmanagement-root.md)политика назначения пакета доступа определяет политику, с помощью которой субъекты могут запрашивать или получать пакет доступа через назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="8e183-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="8e183-106">Пакет доступа может иметь ноль или несколько политик.</span><span class="sxs-lookup"><span data-stu-id="8e183-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="8e183-107">При получении запроса от субъекта тема соедется с каждой политикой, чтобы найти политику (если таково) с requestorSettings, которые включают эту тему.</span><span class="sxs-lookup"><span data-stu-id="8e183-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="8e183-108">Затем политика определяет, требуется ли утверждение запроса, продолжительность назначения пакета доступа и требуется ли регулярно проверять назначение.</span><span class="sxs-lookup"><span data-stu-id="8e183-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="8e183-109">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на пакет доступа и политику назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="8e183-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="8e183-110">Методы</span><span class="sxs-lookup"><span data-stu-id="8e183-110">Methods</span></span>

| <span data-ttu-id="8e183-111">Метод</span><span class="sxs-lookup"><span data-stu-id="8e183-111">Method</span></span>       | <span data-ttu-id="8e183-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e183-112">Return Type</span></span> | <span data-ttu-id="8e183-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8e183-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8e183-114">Список accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="8e183-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="8e183-115">[Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e183-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="8e183-116">Получить список объектов accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e183-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="8e183-117">Создание accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="8e183-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="8e183-119">Создание объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e183-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="8e183-120">Get accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="8e183-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="8e183-122">Чтение свойств и связей объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e183-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="8e183-123">Обновление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="8e183-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="8e183-125">Обновление свойств объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e183-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="8e183-126">Удаление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="8e183-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="8e183-127">Удаление accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e183-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e183-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e183-128">Properties</span></span>

| <span data-ttu-id="8e183-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e183-129">Property</span></span>     | <span data-ttu-id="8e183-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8e183-130">Type</span></span>        | <span data-ttu-id="8e183-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8e183-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e183-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="8e183-132">accessPackageId</span></span>|<span data-ttu-id="8e183-133">String</span><span class="sxs-lookup"><span data-stu-id="8e183-133">String</span></span>|<span data-ttu-id="8e183-134">ИД пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="8e183-134">ID of the access package.</span></span>|
|<span data-ttu-id="8e183-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-135">accessReviewSettings</span></span>|[<span data-ttu-id="8e183-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="8e183-137">Кто должен и как часто проверяются назначения пакета доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="8e183-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="8e183-138">Это свойство имеет null, если проверки не требуются.</span><span class="sxs-lookup"><span data-stu-id="8e183-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="8e183-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="8e183-139">canExtend</span></span>|<span data-ttu-id="8e183-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e183-140">Boolean</span></span>|<span data-ttu-id="8e183-141">Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="8e183-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="8e183-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="8e183-142">createdBy</span></span>|<span data-ttu-id="8e183-143">String</span><span class="sxs-lookup"><span data-stu-id="8e183-143">String</span></span>|<span data-ttu-id="8e183-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e183-144">Read-only.</span></span>|
|<span data-ttu-id="8e183-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e183-145">createdDateTime</span></span>|<span data-ttu-id="8e183-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e183-146">DateTimeOffset</span></span>|<span data-ttu-id="8e183-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e183-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e183-149">description</span><span class="sxs-lookup"><span data-stu-id="8e183-149">description</span></span>|<span data-ttu-id="8e183-150">String</span><span class="sxs-lookup"><span data-stu-id="8e183-150">String</span></span>|<span data-ttu-id="8e183-151">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="8e183-151">The description of the policy.</span></span>|
|<span data-ttu-id="8e183-152">displayName</span><span class="sxs-lookup"><span data-stu-id="8e183-152">displayName</span></span>|<span data-ttu-id="8e183-153">String</span><span class="sxs-lookup"><span data-stu-id="8e183-153">String</span></span>|<span data-ttu-id="8e183-154">Отображаемого имени политики.</span><span class="sxs-lookup"><span data-stu-id="8e183-154">The display name of the policy.</span></span>|
|<span data-ttu-id="8e183-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="8e183-155">durationInDays</span></span>|<span data-ttu-id="8e183-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8e183-156">Int32</span></span>|<span data-ttu-id="8e183-157">Количество дней, в течение которых назначения из этой политики продлятся до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="8e183-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="8e183-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8e183-158">expirationDateTime</span></span>|<span data-ttu-id="8e183-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e183-159">DateTimeOffset</span></span>|<span data-ttu-id="8e183-160">Дата окончания срока действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="8e183-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="8e183-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8e183-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e183-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e183-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e183-163">id</span><span class="sxs-lookup"><span data-stu-id="8e183-163">id</span></span>|<span data-ttu-id="8e183-164">String</span><span class="sxs-lookup"><span data-stu-id="8e183-164">String</span></span>| <span data-ttu-id="8e183-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e183-165">Read-only.</span></span>|
|<span data-ttu-id="8e183-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="8e183-166">modifiedBy</span></span>|<span data-ttu-id="8e183-167">String</span><span class="sxs-lookup"><span data-stu-id="8e183-167">String</span></span>|<span data-ttu-id="8e183-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e183-168">Read-only.</span></span>|
|<span data-ttu-id="8e183-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e183-169">modifiedDateTime</span></span>|<span data-ttu-id="8e183-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e183-170">DateTimeOffset</span></span>|<span data-ttu-id="8e183-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e183-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e183-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-173">requestApprovalSettings</span></span>|[<span data-ttu-id="8e183-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="8e183-175">Кто должен утверждать запросы на пакет доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="8e183-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="8e183-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-176">requestorSettings</span></span>|[<span data-ttu-id="8e183-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="8e183-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="8e183-178">Кто может запросить этот пакет доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="8e183-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="8e183-179">вопросы</span><span class="sxs-lookup"><span data-stu-id="8e183-179">questions</span></span>|<span data-ttu-id="8e183-180">[Коллекция accessPackageQuestion](accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="8e183-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="8e183-181">Вопросы, которые представляют запросителем.</span><span class="sxs-lookup"><span data-stu-id="8e183-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8e183-182">Отношения</span><span class="sxs-lookup"><span data-stu-id="8e183-182">Relationships</span></span>

| <span data-ttu-id="8e183-183">Связь</span><span class="sxs-lookup"><span data-stu-id="8e183-183">Relationship</span></span> | <span data-ttu-id="8e183-184">Тип</span><span class="sxs-lookup"><span data-stu-id="8e183-184">Type</span></span>        | <span data-ttu-id="8e183-185">Описание</span><span class="sxs-lookup"><span data-stu-id="8e183-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e183-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8e183-186">accessPackage</span></span>|[<span data-ttu-id="8e183-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8e183-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="8e183-188">Пакет доступа с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="8e183-188">The access package with this policy.</span></span> <span data-ttu-id="8e183-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e183-189">Read-only.</span></span> <span data-ttu-id="8e183-190">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8e183-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e183-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e183-191">JSON representation</span></span>

<span data-ttu-id="8e183-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e183-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

