---
title: Тип ресурса Акцесспаккажеассигнментполици
description: Политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccf3e1bb94bb1f6186e39cdaa91fa2dbe3a4344d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031739"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="77502-103">Тип ресурса Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="77502-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77502-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77502-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="77502-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="77502-106">Пакет Access может иметь не более одного или нескольких политик.</span><span class="sxs-lookup"><span data-stu-id="77502-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="77502-107">При получении запроса от субъекта субъект сравнивается с каждой политикой, чтобы найти политику (если она есть) с Рекуесторсеттингс, включающей в себя эту тему.</span><span class="sxs-lookup"><span data-stu-id="77502-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="77502-108">После этого политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета Access, а также должно ли назначение регулярно проверяться.</span><span class="sxs-lookup"><span data-stu-id="77502-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="77502-109">Чтобы назначить пользователя пакету доступа, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , который ссылается на политику назначения пакетов доступа и пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="77502-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="77502-110">Методы</span><span class="sxs-lookup"><span data-stu-id="77502-110">Methods</span></span>

| <span data-ttu-id="77502-111">Метод</span><span class="sxs-lookup"><span data-stu-id="77502-111">Method</span></span>       | <span data-ttu-id="77502-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77502-112">Return Type</span></span> | <span data-ttu-id="77502-113">Описание</span><span class="sxs-lookup"><span data-stu-id="77502-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77502-114">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="77502-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="77502-115">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77502-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="77502-116">Получение списка объектов Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="77502-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="77502-117">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="77502-118">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="77502-119">Создание нового объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="77502-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="77502-120">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="77502-121">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="77502-122">Чтение свойств и связей объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="77502-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="77502-123">Обновление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="77502-124">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="77502-125">Обновление свойств объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="77502-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="77502-126">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="77502-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="77502-127">Удаление Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="77502-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="77502-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="77502-128">Properties</span></span>

| <span data-ttu-id="77502-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77502-129">Property</span></span>     | <span data-ttu-id="77502-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77502-130">Type</span></span>        | <span data-ttu-id="77502-131">Описание</span><span class="sxs-lookup"><span data-stu-id="77502-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77502-132">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="77502-132">accessPackageId</span></span>|<span data-ttu-id="77502-133">String</span><span class="sxs-lookup"><span data-stu-id="77502-133">String</span></span>|<span data-ttu-id="77502-134">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="77502-134">ID of the access package.</span></span>|
|<span data-ttu-id="77502-135">акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-135">accessReviewSettings</span></span>|[<span data-ttu-id="77502-136">ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="77502-137">Кто должен проверить и как часто назначений для пакета доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="77502-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="77502-138">Это свойство имеет значение null, если проверка не требуются.</span><span class="sxs-lookup"><span data-stu-id="77502-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="77502-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="77502-139">canExtend</span></span>|<span data-ttu-id="77502-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="77502-140">Boolean</span></span>|<span data-ttu-id="77502-141">Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="77502-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="77502-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="77502-142">createdBy</span></span>|<span data-ttu-id="77502-143">String</span><span class="sxs-lookup"><span data-stu-id="77502-143">String</span></span>|<span data-ttu-id="77502-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77502-144">Read-only.</span></span>|
|<span data-ttu-id="77502-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77502-145">createdDateTime</span></span>|<span data-ttu-id="77502-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77502-146">DateTimeOffset</span></span>|<span data-ttu-id="77502-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77502-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77502-149">description</span><span class="sxs-lookup"><span data-stu-id="77502-149">description</span></span>|<span data-ttu-id="77502-150">String</span><span class="sxs-lookup"><span data-stu-id="77502-150">String</span></span>|<span data-ttu-id="77502-151">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="77502-151">The description of the policy.</span></span>|
|<span data-ttu-id="77502-152">displayName</span><span class="sxs-lookup"><span data-stu-id="77502-152">displayName</span></span>|<span data-ttu-id="77502-153">String</span><span class="sxs-lookup"><span data-stu-id="77502-153">String</span></span>|<span data-ttu-id="77502-154">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="77502-154">The display name of the policy.</span></span>|
|<span data-ttu-id="77502-155">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="77502-155">durationInDays</span></span>|<span data-ttu-id="77502-156">Int32</span><span class="sxs-lookup"><span data-stu-id="77502-156">Int32</span></span>|<span data-ttu-id="77502-157">Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="77502-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="77502-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77502-158">expirationDateTime</span></span>|<span data-ttu-id="77502-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77502-159">DateTimeOffset</span></span>|<span data-ttu-id="77502-160">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="77502-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="77502-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="77502-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77502-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77502-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77502-163">id</span><span class="sxs-lookup"><span data-stu-id="77502-163">id</span></span>|<span data-ttu-id="77502-164">String</span><span class="sxs-lookup"><span data-stu-id="77502-164">String</span></span>| <span data-ttu-id="77502-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77502-165">Read-only.</span></span>|
|<span data-ttu-id="77502-166">модифиедби</span><span class="sxs-lookup"><span data-stu-id="77502-166">modifiedBy</span></span>|<span data-ttu-id="77502-167">String</span><span class="sxs-lookup"><span data-stu-id="77502-167">String</span></span>|<span data-ttu-id="77502-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77502-168">Read-only.</span></span>|
|<span data-ttu-id="77502-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77502-169">modifiedDateTime</span></span>|<span data-ttu-id="77502-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77502-170">DateTimeOffset</span></span>|<span data-ttu-id="77502-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77502-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77502-173">рекуестаппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-173">requestApprovalSettings</span></span>|[<span data-ttu-id="77502-174">аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="77502-175">Кто должен утверждать запросы на пакет Access в этой политике.</span><span class="sxs-lookup"><span data-stu-id="77502-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="77502-176">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-176">requestorSettings</span></span>|[<span data-ttu-id="77502-177">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="77502-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="77502-178">Кто может запрашивать этот пакет Access из этой политики.</span><span class="sxs-lookup"><span data-stu-id="77502-178">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="77502-179">Связи</span><span class="sxs-lookup"><span data-stu-id="77502-179">Relationships</span></span>

| <span data-ttu-id="77502-180">Связь</span><span class="sxs-lookup"><span data-stu-id="77502-180">Relationship</span></span> | <span data-ttu-id="77502-181">Тип</span><span class="sxs-lookup"><span data-stu-id="77502-181">Type</span></span>        | <span data-ttu-id="77502-182">Описание</span><span class="sxs-lookup"><span data-stu-id="77502-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77502-183">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="77502-183">accessPackage</span></span>|[<span data-ttu-id="77502-184">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="77502-184">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="77502-185">Пакет Access с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="77502-185">The access package with this policy.</span></span> <span data-ttu-id="77502-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77502-186">Read-only.</span></span> <span data-ttu-id="77502-187">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="77502-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77502-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77502-188">JSON representation</span></span>

<span data-ttu-id="77502-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77502-189">The following is a JSON representation of the resource.</span></span>

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


