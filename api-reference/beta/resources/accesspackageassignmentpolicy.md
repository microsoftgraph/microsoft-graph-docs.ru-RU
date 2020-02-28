---
title: Тип ресурса Акцесспаккажеассигнментполици
description: Политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08fcefafe9a354a57415a7d05bee1ec57ffdc138
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331306"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="9dc4d-103">Тип ресурса Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc4d-104">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="9dc4d-105">Пакет Access может иметь не более одного или нескольких политик.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="9dc4d-106">При получении запроса от субъекта субъект сравнивается с каждой политикой, чтобы найти политику (если она есть) с Рекуесторсеттингс, включающей в себя эту тему.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="9dc4d-107">После этого политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета Access, а также должно ли назначение регулярно проверяться.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-107">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="9dc4d-108">Чтобы назначить пользователя пакету доступа, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , который ссылается на политику назначения пакетов доступа и пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="9dc4d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="9dc4d-109">Methods</span></span>

| <span data-ttu-id="9dc4d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="9dc4d-110">Method</span></span>       | <span data-ttu-id="9dc4d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9dc4d-111">Return Type</span></span> | <span data-ttu-id="9dc4d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc4d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9dc4d-113">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="9dc4d-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="9dc4d-114">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dc4d-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="9dc4d-115">Получение списка объектов Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="9dc4d-116">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="9dc4d-117">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="9dc4d-118">Создание нового объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="9dc4d-119">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="9dc4d-120">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="9dc4d-121">Чтение свойств и связей объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="9dc4d-122">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="9dc4d-123">Удаление Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="9dc4d-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dc4d-124">Properties</span></span>

| <span data-ttu-id="9dc4d-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dc4d-125">Property</span></span>     | <span data-ttu-id="9dc4d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc4d-126">Type</span></span>        | <span data-ttu-id="9dc4d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc4d-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9dc4d-128">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="9dc4d-128">accessPackageId</span></span>|<span data-ttu-id="9dc4d-129">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-129">String</span></span>|<span data-ttu-id="9dc4d-130">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-130">ID of the access package.</span></span>|
|<span data-ttu-id="9dc4d-131">акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-131">accessReviewSettings</span></span>|[<span data-ttu-id="9dc4d-132">ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-132">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="9dc4d-133">Кто должен проверить и как часто назначений для пакета доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-133">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="9dc4d-134">Это свойство имеет значение null, если проверка не требуются.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-134">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="9dc4d-135">canExtend</span><span class="sxs-lookup"><span data-stu-id="9dc4d-135">canExtend</span></span>|<span data-ttu-id="9dc4d-136">Логический</span><span class="sxs-lookup"><span data-stu-id="9dc4d-136">Boolean</span></span>|<span data-ttu-id="9dc4d-137">Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-137">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="9dc4d-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="9dc4d-138">createdBy</span></span>|<span data-ttu-id="9dc4d-139">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-139">String</span></span>|<span data-ttu-id="9dc4d-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-140">Read-only.</span></span>|
|<span data-ttu-id="9dc4d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc4d-141">createdDateTime</span></span>|<span data-ttu-id="9dc4d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc4d-142">DateTimeOffset</span></span>|<span data-ttu-id="9dc4d-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9dc4d-145">description</span><span class="sxs-lookup"><span data-stu-id="9dc4d-145">description</span></span>|<span data-ttu-id="9dc4d-146">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-146">String</span></span>|<span data-ttu-id="9dc4d-147">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-147">The description of the policy.</span></span>|
|<span data-ttu-id="9dc4d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9dc4d-148">displayName</span></span>|<span data-ttu-id="9dc4d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="9dc4d-149">String</span></span>|<span data-ttu-id="9dc4d-150">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-150">The display name of the policy.</span></span>|
|<span data-ttu-id="9dc4d-151">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-151">durationInDays</span></span>|<span data-ttu-id="9dc4d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9dc4d-152">Int32</span></span>|<span data-ttu-id="9dc4d-153">Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-153">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="9dc4d-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc4d-154">expirationDateTime</span></span>|<span data-ttu-id="9dc4d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc4d-155">DateTimeOffset</span></span>|<span data-ttu-id="9dc4d-156">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-156">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="9dc4d-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9dc4d-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9dc4d-158">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9dc4d-159">id</span><span class="sxs-lookup"><span data-stu-id="9dc4d-159">id</span></span>|<span data-ttu-id="9dc4d-160">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-160">String</span></span>| <span data-ttu-id="9dc4d-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-161">Read-only.</span></span>|
|<span data-ttu-id="9dc4d-162">исдениполици</span><span class="sxs-lookup"><span data-stu-id="9dc4d-162">isDenyPolicy</span></span>|<span data-ttu-id="9dc4d-163">Логический</span><span class="sxs-lookup"><span data-stu-id="9dc4d-163">Boolean</span></span>|<span data-ttu-id="9dc4d-164">Если этот параметр имеет значение true, доступ не будет разрешен.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-164">If true, the policy will not permit access.</span></span> <span data-ttu-id="9dc4d-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-165">Read only.</span></span>|
|<span data-ttu-id="9dc4d-166">модифиедби</span><span class="sxs-lookup"><span data-stu-id="9dc4d-166">modifiedBy</span></span>|<span data-ttu-id="9dc4d-167">String</span><span class="sxs-lookup"><span data-stu-id="9dc4d-167">String</span></span>|<span data-ttu-id="9dc4d-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-168">Read-only.</span></span>|
|<span data-ttu-id="9dc4d-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc4d-169">modifiedDateTime</span></span>|<span data-ttu-id="9dc4d-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc4d-170">DateTimeOffset</span></span>|<span data-ttu-id="9dc4d-p106">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9dc4d-173">рекуестаппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-173">requestApprovalSettings</span></span>|[<span data-ttu-id="9dc4d-174">аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="9dc4d-175">Кто должен утверждать запросы на пакет Access в этой политике.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="9dc4d-176">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-176">requestorSettings</span></span>|[<span data-ttu-id="9dc4d-177">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dc4d-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="9dc4d-178">Кто может запрашивать этот пакет Access из этой политики.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-178">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="9dc4d-179">Связи</span><span class="sxs-lookup"><span data-stu-id="9dc4d-179">Relationships</span></span>

| <span data-ttu-id="9dc4d-180">Связь</span><span class="sxs-lookup"><span data-stu-id="9dc4d-180">Relationship</span></span> | <span data-ttu-id="9dc4d-181">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc4d-181">Type</span></span>        | <span data-ttu-id="9dc4d-182">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc4d-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9dc4d-183">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="9dc4d-183">accessPackage</span></span>|[<span data-ttu-id="9dc4d-184">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="9dc4d-184">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="9dc4d-185">Пакет Access с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-185">The access package with this policy.</span></span> <span data-ttu-id="9dc4d-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-186">Read-only.</span></span> <span data-ttu-id="9dc4d-187">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dc4d-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dc4d-188">JSON representation</span></span>

<span data-ttu-id="9dc4d-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dc4d-189">The following is a JSON representation of the resource.</span></span>

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
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings" : {
      "scopeType": "AllExistingDirectorySubjects",
      "acceptRequests": true,
      "allowedRequestors": []
    },
    "requestApprovalSettings" : {
      "isApprovalRequired": false,
      "isApprovalRequiredForExtension": false,
      "isRequestorJustificationRequired": false,
      "approvalMode": "NoApproval",
      "approvalStages": []
    },
    "accessReviewSettings" : null
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
