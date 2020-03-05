---
title: Тип ресурса Акцесспаккажеассигнментполици
description: Политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dd70512db17df29685c4af2d8aa4c410a78642b0
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534441"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="180c3-103">Тип ресурса Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="180c3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="180c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180c3-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="180c3-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="180c3-106">Пакет Access может иметь не более одного или нескольких политик.</span><span class="sxs-lookup"><span data-stu-id="180c3-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="180c3-107">При получении запроса от субъекта субъект сравнивается с каждой политикой, чтобы найти политику (если она есть) с Рекуесторсеттингс, включающей в себя эту тему.</span><span class="sxs-lookup"><span data-stu-id="180c3-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="180c3-108">После этого политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета Access, а также должно ли назначение регулярно проверяться.</span><span class="sxs-lookup"><span data-stu-id="180c3-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="180c3-109">Чтобы назначить пользователя пакету доступа, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , который ссылается на политику назначения пакетов доступа и пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="180c3-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="180c3-110">Методы</span><span class="sxs-lookup"><span data-stu-id="180c3-110">Methods</span></span>

| <span data-ttu-id="180c3-111">Метод</span><span class="sxs-lookup"><span data-stu-id="180c3-111">Method</span></span>       | <span data-ttu-id="180c3-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="180c3-112">Return Type</span></span> | <span data-ttu-id="180c3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="180c3-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="180c3-114">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="180c3-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="180c3-115">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="180c3-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="180c3-116">Получение списка объектов Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="180c3-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="180c3-117">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="180c3-118">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="180c3-119">Создание нового объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="180c3-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="180c3-120">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="180c3-121">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="180c3-122">Чтение свойств и связей объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="180c3-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="180c3-123">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="180c3-123">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="180c3-124">Удаление Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="180c3-124">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="180c3-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="180c3-125">Properties</span></span>

| <span data-ttu-id="180c3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="180c3-126">Property</span></span>     | <span data-ttu-id="180c3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="180c3-127">Type</span></span>        | <span data-ttu-id="180c3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="180c3-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="180c3-129">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="180c3-129">accessPackageId</span></span>|<span data-ttu-id="180c3-130">String</span><span class="sxs-lookup"><span data-stu-id="180c3-130">String</span></span>|<span data-ttu-id="180c3-131">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="180c3-131">ID of the access package.</span></span>|
|<span data-ttu-id="180c3-132">акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-132">accessReviewSettings</span></span>|[<span data-ttu-id="180c3-133">ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-133">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="180c3-134">Кто должен проверить и как часто назначений для пакета доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="180c3-134">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="180c3-135">Это свойство имеет значение null, если проверка не требуются.</span><span class="sxs-lookup"><span data-stu-id="180c3-135">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="180c3-136">canExtend</span><span class="sxs-lookup"><span data-stu-id="180c3-136">canExtend</span></span>|<span data-ttu-id="180c3-137">Логический</span><span class="sxs-lookup"><span data-stu-id="180c3-137">Boolean</span></span>|<span data-ttu-id="180c3-138">Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="180c3-138">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="180c3-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="180c3-139">createdBy</span></span>|<span data-ttu-id="180c3-140">String</span><span class="sxs-lookup"><span data-stu-id="180c3-140">String</span></span>|<span data-ttu-id="180c3-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180c3-141">Read-only.</span></span>|
|<span data-ttu-id="180c3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="180c3-142">createdDateTime</span></span>|<span data-ttu-id="180c3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180c3-143">DateTimeOffset</span></span>|<span data-ttu-id="180c3-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="180c3-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="180c3-146">description</span><span class="sxs-lookup"><span data-stu-id="180c3-146">description</span></span>|<span data-ttu-id="180c3-147">String</span><span class="sxs-lookup"><span data-stu-id="180c3-147">String</span></span>|<span data-ttu-id="180c3-148">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="180c3-148">The description of the policy.</span></span>|
|<span data-ttu-id="180c3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="180c3-149">displayName</span></span>|<span data-ttu-id="180c3-150">Строка</span><span class="sxs-lookup"><span data-stu-id="180c3-150">String</span></span>|<span data-ttu-id="180c3-151">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="180c3-151">The display name of the policy.</span></span>|
|<span data-ttu-id="180c3-152">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="180c3-152">durationInDays</span></span>|<span data-ttu-id="180c3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="180c3-153">Int32</span></span>|<span data-ttu-id="180c3-154">Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="180c3-154">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="180c3-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="180c3-155">expirationDateTime</span></span>|<span data-ttu-id="180c3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180c3-156">DateTimeOffset</span></span>|<span data-ttu-id="180c3-157">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="180c3-157">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="180c3-158">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="180c3-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="180c3-159">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="180c3-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="180c3-160">id</span><span class="sxs-lookup"><span data-stu-id="180c3-160">id</span></span>|<span data-ttu-id="180c3-161">String</span><span class="sxs-lookup"><span data-stu-id="180c3-161">String</span></span>| <span data-ttu-id="180c3-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180c3-162">Read-only.</span></span>|
|<span data-ttu-id="180c3-163">модифиедби</span><span class="sxs-lookup"><span data-stu-id="180c3-163">modifiedBy</span></span>|<span data-ttu-id="180c3-164">String</span><span class="sxs-lookup"><span data-stu-id="180c3-164">String</span></span>|<span data-ttu-id="180c3-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180c3-165">Read-only.</span></span>|
|<span data-ttu-id="180c3-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="180c3-166">modifiedDateTime</span></span>|<span data-ttu-id="180c3-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180c3-167">DateTimeOffset</span></span>|<span data-ttu-id="180c3-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="180c3-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="180c3-170">рекуестаппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-170">requestApprovalSettings</span></span>|[<span data-ttu-id="180c3-171">аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-171">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="180c3-172">Кто должен утверждать запросы на пакет Access в этой политике.</span><span class="sxs-lookup"><span data-stu-id="180c3-172">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="180c3-173">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-173">requestorSettings</span></span>|[<span data-ttu-id="180c3-174">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="180c3-174">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="180c3-175">Кто может запрашивать этот пакет Access из этой политики.</span><span class="sxs-lookup"><span data-stu-id="180c3-175">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="180c3-176">Связи</span><span class="sxs-lookup"><span data-stu-id="180c3-176">Relationships</span></span>

| <span data-ttu-id="180c3-177">Связь</span><span class="sxs-lookup"><span data-stu-id="180c3-177">Relationship</span></span> | <span data-ttu-id="180c3-178">Тип</span><span class="sxs-lookup"><span data-stu-id="180c3-178">Type</span></span>        | <span data-ttu-id="180c3-179">Описание</span><span class="sxs-lookup"><span data-stu-id="180c3-179">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="180c3-180">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="180c3-180">accessPackage</span></span>|[<span data-ttu-id="180c3-181">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="180c3-181">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="180c3-182">Пакет Access с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="180c3-182">The access package with this policy.</span></span> <span data-ttu-id="180c3-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180c3-183">Read-only.</span></span> <span data-ttu-id="180c3-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="180c3-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="180c3-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="180c3-185">JSON representation</span></span>

<span data-ttu-id="180c3-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="180c3-186">The following is a JSON representation of the resource.</span></span>

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
