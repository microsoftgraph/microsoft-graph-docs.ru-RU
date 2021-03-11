---
title: тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db463609803e3547b88f586cc447974846738e22
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720454"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="47c89-103">тип ресурса accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="47c89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47c89-105">В управлении правами [Azure AD](entitlementmanagement-root.md)политика назначения пакетов доступа указывает политику, в которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="47c89-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="47c89-106">Пакет доступа может иметь нулевую или несколько политик.</span><span class="sxs-lookup"><span data-stu-id="47c89-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="47c89-107">При получении запроса субъекта субъекту соответствует каждая политика, чтобы найти политику (если таково) с requestorSettings, которые включают этот субъект.</span><span class="sxs-lookup"><span data-stu-id="47c89-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="47c89-108">Затем политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета доступа и требуется ли регулярное рассмотрение назначения.</span><span class="sxs-lookup"><span data-stu-id="47c89-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="47c89-109">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на политику назначения пакета доступа и пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="47c89-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="47c89-110">Методы</span><span class="sxs-lookup"><span data-stu-id="47c89-110">Methods</span></span>

| <span data-ttu-id="47c89-111">Метод</span><span class="sxs-lookup"><span data-stu-id="47c89-111">Method</span></span>       | <span data-ttu-id="47c89-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47c89-112">Return Type</span></span> | <span data-ttu-id="47c89-113">Описание</span><span class="sxs-lookup"><span data-stu-id="47c89-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="47c89-114">Список accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="47c89-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="47c89-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span><span class="sxs-lookup"><span data-stu-id="47c89-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="47c89-116">Извлечение списка объектов accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="47c89-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="47c89-117">Создание accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="47c89-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="47c89-119">Создание нового объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="47c89-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="47c89-120">Получить accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="47c89-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="47c89-122">Чтение свойств и связей объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="47c89-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="47c89-123">Обновление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="47c89-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="47c89-125">Обновление свойств объекта accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="47c89-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="47c89-126">Удаление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="47c89-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="47c89-127">Удаление accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="47c89-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="47c89-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="47c89-128">Properties</span></span>

| <span data-ttu-id="47c89-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="47c89-129">Property</span></span>     | <span data-ttu-id="47c89-130">Тип</span><span class="sxs-lookup"><span data-stu-id="47c89-130">Type</span></span>        | <span data-ttu-id="47c89-131">Описание</span><span class="sxs-lookup"><span data-stu-id="47c89-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47c89-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="47c89-132">accessPackageId</span></span>|<span data-ttu-id="47c89-133">String</span><span class="sxs-lookup"><span data-stu-id="47c89-133">String</span></span>|<span data-ttu-id="47c89-134">ID пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="47c89-134">ID of the access package.</span></span>|
|<span data-ttu-id="47c89-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-135">accessReviewSettings</span></span>|[<span data-ttu-id="47c89-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="47c89-137">Кто должен и как часто выполнять назначения пакету доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="47c89-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="47c89-138">Это свойство является null, если отзывы не требуются.</span><span class="sxs-lookup"><span data-stu-id="47c89-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="47c89-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="47c89-139">canExtend</span></span>|<span data-ttu-id="47c89-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="47c89-140">Boolean</span></span>|<span data-ttu-id="47c89-141">Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="47c89-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="47c89-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="47c89-142">createdBy</span></span>|<span data-ttu-id="47c89-143">String</span><span class="sxs-lookup"><span data-stu-id="47c89-143">String</span></span>|<span data-ttu-id="47c89-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c89-144">Read-only.</span></span>|
|<span data-ttu-id="47c89-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47c89-145">createdDateTime</span></span>|<span data-ttu-id="47c89-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c89-146">DateTimeOffset</span></span>|<span data-ttu-id="47c89-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="47c89-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47c89-148">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="47c89-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="47c89-149">description</span><span class="sxs-lookup"><span data-stu-id="47c89-149">description</span></span>|<span data-ttu-id="47c89-150">String</span><span class="sxs-lookup"><span data-stu-id="47c89-150">String</span></span>|<span data-ttu-id="47c89-151">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="47c89-151">The description of the policy.</span></span>|
|<span data-ttu-id="47c89-152">displayName</span><span class="sxs-lookup"><span data-stu-id="47c89-152">displayName</span></span>|<span data-ttu-id="47c89-153">String</span><span class="sxs-lookup"><span data-stu-id="47c89-153">String</span></span>|<span data-ttu-id="47c89-154">Отображает имя политики.</span><span class="sxs-lookup"><span data-stu-id="47c89-154">The display name of the policy.</span></span>|
|<span data-ttu-id="47c89-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="47c89-155">durationInDays</span></span>|<span data-ttu-id="47c89-156">Int32</span><span class="sxs-lookup"><span data-stu-id="47c89-156">Int32</span></span>|<span data-ttu-id="47c89-157">Количество дней, в течение которых назначения из этой политики будут выполняться до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="47c89-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="47c89-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="47c89-158">expirationDateTime</span></span>|<span data-ttu-id="47c89-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c89-159">DateTimeOffset</span></span>|<span data-ttu-id="47c89-160">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="47c89-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="47c89-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="47c89-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47c89-162">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="47c89-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="47c89-163">id</span><span class="sxs-lookup"><span data-stu-id="47c89-163">id</span></span>|<span data-ttu-id="47c89-164">String</span><span class="sxs-lookup"><span data-stu-id="47c89-164">String</span></span>| <span data-ttu-id="47c89-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c89-165">Read-only.</span></span>|
|<span data-ttu-id="47c89-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="47c89-166">modifiedBy</span></span>|<span data-ttu-id="47c89-167">String</span><span class="sxs-lookup"><span data-stu-id="47c89-167">String</span></span>|<span data-ttu-id="47c89-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c89-168">Read-only.</span></span>|
|<span data-ttu-id="47c89-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47c89-169">modifiedDateTime</span></span>|<span data-ttu-id="47c89-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c89-170">DateTimeOffset</span></span>|<span data-ttu-id="47c89-171">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="47c89-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47c89-172">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="47c89-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="47c89-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-173">requestApprovalSettings</span></span>|[<span data-ttu-id="47c89-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="47c89-175">Кто должен утверждать запросы на пакет доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="47c89-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="47c89-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-176">requestorSettings</span></span>|[<span data-ttu-id="47c89-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="47c89-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="47c89-178">Кто может запросить этот пакет доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="47c89-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="47c89-179">вопросы</span><span class="sxs-lookup"><span data-stu-id="47c89-179">questions</span></span>|<span data-ttu-id="47c89-180">[коллекция accessPackageQuestion](accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="47c89-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="47c89-181">Вопросы, заданные запросчику.</span><span class="sxs-lookup"><span data-stu-id="47c89-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="47c89-182">Связи</span><span class="sxs-lookup"><span data-stu-id="47c89-182">Relationships</span></span>

| <span data-ttu-id="47c89-183">Связь</span><span class="sxs-lookup"><span data-stu-id="47c89-183">Relationship</span></span> | <span data-ttu-id="47c89-184">Тип</span><span class="sxs-lookup"><span data-stu-id="47c89-184">Type</span></span>        | <span data-ttu-id="47c89-185">Описание</span><span class="sxs-lookup"><span data-stu-id="47c89-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47c89-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="47c89-186">accessPackage</span></span>|[<span data-ttu-id="47c89-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="47c89-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="47c89-188">Пакет доступа с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="47c89-188">The access package with this policy.</span></span> <span data-ttu-id="47c89-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c89-189">Read-only.</span></span> <span data-ttu-id="47c89-190">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="47c89-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47c89-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47c89-191">JSON representation</span></span>

<span data-ttu-id="47c89-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47c89-192">The following is a JSON representation of the resource.</span></span>

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

