---
title: тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 269a3a27d83951c82d50dcaf0ba52c6ce7a5a1bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433285"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="08a27-103">тип ресурса accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="08a27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08a27-105">В управлении правами [Azure AD](entitlementmanagement-root.md)политика назначения пакетов доступа указывает политику, в которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="08a27-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="08a27-106">Пакет доступа может иметь нулевую или несколько политик.</span><span class="sxs-lookup"><span data-stu-id="08a27-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="08a27-107">При получении запроса субъекта субъекту соответствует каждая политика, чтобы найти политику (если таково) с requestorSettings, которые включают этот субъект.</span><span class="sxs-lookup"><span data-stu-id="08a27-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="08a27-108">Затем политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета доступа и требуется ли регулярное рассмотрение назначения.</span><span class="sxs-lookup"><span data-stu-id="08a27-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="08a27-109">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на политику назначения пакета доступа и пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="08a27-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="08a27-110">Методы</span><span class="sxs-lookup"><span data-stu-id="08a27-110">Methods</span></span>

| <span data-ttu-id="08a27-111">Метод</span><span class="sxs-lookup"><span data-stu-id="08a27-111">Method</span></span>       | <span data-ttu-id="08a27-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08a27-112">Return Type</span></span> | <span data-ttu-id="08a27-113">Описание</span><span class="sxs-lookup"><span data-stu-id="08a27-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="08a27-114">Список accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="08a27-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="08a27-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span><span class="sxs-lookup"><span data-stu-id="08a27-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="08a27-116">Извлечение списка объектов accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="08a27-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="08a27-117">Создание accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="08a27-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="08a27-119">Создание нового объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="08a27-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="08a27-120">Получить accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="08a27-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="08a27-122">Чтение свойств и связей объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="08a27-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="08a27-123">Обновление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="08a27-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="08a27-125">Обновление свойств объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="08a27-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="08a27-126">Удаление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="08a27-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="08a27-127">Удаление accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="08a27-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="08a27-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="08a27-128">Properties</span></span>

| <span data-ttu-id="08a27-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08a27-129">Property</span></span>     | <span data-ttu-id="08a27-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08a27-130">Type</span></span>        | <span data-ttu-id="08a27-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08a27-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08a27-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="08a27-132">accessPackageId</span></span>|<span data-ttu-id="08a27-133">String</span><span class="sxs-lookup"><span data-stu-id="08a27-133">String</span></span>|<span data-ttu-id="08a27-134">ID пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="08a27-134">ID of the access package.</span></span>|
|<span data-ttu-id="08a27-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-135">accessReviewSettings</span></span>|[<span data-ttu-id="08a27-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="08a27-137">Кто должен и как часто выполнять назначения пакету доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="08a27-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="08a27-138">Это свойство является null, если отзывы не требуются.</span><span class="sxs-lookup"><span data-stu-id="08a27-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="08a27-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="08a27-139">canExtend</span></span>|<span data-ttu-id="08a27-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a27-140">Boolean</span></span>|<span data-ttu-id="08a27-141">Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="08a27-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="08a27-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="08a27-142">createdBy</span></span>|<span data-ttu-id="08a27-143">String</span><span class="sxs-lookup"><span data-stu-id="08a27-143">String</span></span>|<span data-ttu-id="08a27-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08a27-144">Read-only.</span></span>|
|<span data-ttu-id="08a27-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08a27-145">createdDateTime</span></span>|<span data-ttu-id="08a27-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a27-146">DateTimeOffset</span></span>|<span data-ttu-id="08a27-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08a27-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08a27-149">description</span><span class="sxs-lookup"><span data-stu-id="08a27-149">description</span></span>|<span data-ttu-id="08a27-150">String</span><span class="sxs-lookup"><span data-stu-id="08a27-150">String</span></span>|<span data-ttu-id="08a27-151">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="08a27-151">The description of the policy.</span></span>|
|<span data-ttu-id="08a27-152">displayName</span><span class="sxs-lookup"><span data-stu-id="08a27-152">displayName</span></span>|<span data-ttu-id="08a27-153">String</span><span class="sxs-lookup"><span data-stu-id="08a27-153">String</span></span>|<span data-ttu-id="08a27-154">Отображает имя политики.</span><span class="sxs-lookup"><span data-stu-id="08a27-154">The display name of the policy.</span></span>|
|<span data-ttu-id="08a27-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="08a27-155">durationInDays</span></span>|<span data-ttu-id="08a27-156">Int32</span><span class="sxs-lookup"><span data-stu-id="08a27-156">Int32</span></span>|<span data-ttu-id="08a27-157">Количество дней, в течение которых назначения из этой политики будут выполняться до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="08a27-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="08a27-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08a27-158">expirationDateTime</span></span>|<span data-ttu-id="08a27-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a27-159">DateTimeOffset</span></span>|<span data-ttu-id="08a27-160">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="08a27-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="08a27-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="08a27-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08a27-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08a27-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08a27-163">id</span><span class="sxs-lookup"><span data-stu-id="08a27-163">id</span></span>|<span data-ttu-id="08a27-164">String</span><span class="sxs-lookup"><span data-stu-id="08a27-164">String</span></span>| <span data-ttu-id="08a27-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08a27-165">Read-only.</span></span>|
|<span data-ttu-id="08a27-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="08a27-166">modifiedBy</span></span>|<span data-ttu-id="08a27-167">String</span><span class="sxs-lookup"><span data-stu-id="08a27-167">String</span></span>|<span data-ttu-id="08a27-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08a27-168">Read-only.</span></span>|
|<span data-ttu-id="08a27-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08a27-169">modifiedDateTime</span></span>|<span data-ttu-id="08a27-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08a27-170">DateTimeOffset</span></span>|<span data-ttu-id="08a27-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08a27-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08a27-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-173">requestApprovalSettings</span></span>|[<span data-ttu-id="08a27-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="08a27-175">Кто должен утверждать запросы на пакет доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="08a27-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="08a27-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-176">requestorSettings</span></span>|[<span data-ttu-id="08a27-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="08a27-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="08a27-178">Кто может запросить этот пакет доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="08a27-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="08a27-179">вопросы</span><span class="sxs-lookup"><span data-stu-id="08a27-179">questions</span></span>|<span data-ttu-id="08a27-180">[коллекция accessPackageQuestion](accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="08a27-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="08a27-181">Вопросы, заданные запросчику.</span><span class="sxs-lookup"><span data-stu-id="08a27-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="08a27-182">Связи</span><span class="sxs-lookup"><span data-stu-id="08a27-182">Relationships</span></span>

| <span data-ttu-id="08a27-183">Связь</span><span class="sxs-lookup"><span data-stu-id="08a27-183">Relationship</span></span> | <span data-ttu-id="08a27-184">Тип</span><span class="sxs-lookup"><span data-stu-id="08a27-184">Type</span></span>        | <span data-ttu-id="08a27-185">Описание</span><span class="sxs-lookup"><span data-stu-id="08a27-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08a27-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="08a27-186">accessPackage</span></span>|[<span data-ttu-id="08a27-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="08a27-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="08a27-188">Пакет доступа с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="08a27-188">The access package with this policy.</span></span> <span data-ttu-id="08a27-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08a27-189">Read-only.</span></span> <span data-ttu-id="08a27-190">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="08a27-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08a27-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08a27-191">JSON representation</span></span>

<span data-ttu-id="08a27-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08a27-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
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

