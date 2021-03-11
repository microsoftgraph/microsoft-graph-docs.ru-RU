---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e188857a2cc92210d9298d588c7d411e16fb688a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720286"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="b4553-103">тип ресурса accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="b4553-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="b4553-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4553-105">В [управлении правами Azure AD](entitlementmanagement-root.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту на определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="b4553-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="b4553-106">Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.</span><span class="sxs-lookup"><span data-stu-id="b4553-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="b4553-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b4553-107">Methods</span></span>

| <span data-ttu-id="b4553-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b4553-108">Method</span></span>       | <span data-ttu-id="b4553-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b4553-109">Return Type</span></span> | <span data-ttu-id="b4553-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4553-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b4553-111">Списки accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="b4553-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="b4553-112">[коллекция accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b4553-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="b4553-113">Извлечение списка **объектов accesspackageassignment.**</span><span class="sxs-lookup"><span data-stu-id="b4553-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="b4553-114">**Примечание:** Вы не можете использовать метод для создания или удаления назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="b4553-115">Вместо этого клиент, который хочет запросить назначение пакета доступа для пользователя или удалить назначение пакета доступа у пользователя, может создать [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="b4553-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4553-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4553-116">Properties</span></span>

| <span data-ttu-id="b4553-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4553-117">Property</span></span>     | <span data-ttu-id="b4553-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b4553-118">Type</span></span>        | <span data-ttu-id="b4553-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b4553-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4553-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="b4553-120">accessPackageId</span></span>|<span data-ttu-id="b4553-121">String</span><span class="sxs-lookup"><span data-stu-id="b4553-121">String</span></span>|<span data-ttu-id="b4553-122">Идентификатор пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-122">The identifier of the access package.</span></span> <span data-ttu-id="b4553-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-123">Read-only.</span></span>|
|<span data-ttu-id="b4553-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="b4553-124">assignmentPolicyId</span></span>|<span data-ttu-id="b4553-125">String</span><span class="sxs-lookup"><span data-stu-id="b4553-125">String</span></span>|<span data-ttu-id="b4553-126">Идентификатор политики назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="b4553-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-127">Read-only.</span></span>|
|<span data-ttu-id="b4553-128">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b4553-128">assignmentState</span></span>|<span data-ttu-id="b4553-129">String</span><span class="sxs-lookup"><span data-stu-id="b4553-129">String</span></span>|<span data-ttu-id="b4553-130">Состояние назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-130">The state of the access package assignment.</span></span> <span data-ttu-id="b4553-131">Возможные значения `Delivering` , `Delivered` или `Expired` .</span><span class="sxs-lookup"><span data-stu-id="b4553-131">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="b4553-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-132">Read-only.</span></span>|
|<span data-ttu-id="b4553-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="b4553-133">assignmentStatus</span></span>|<span data-ttu-id="b4553-134">String</span><span class="sxs-lookup"><span data-stu-id="b4553-134">String</span></span>|<span data-ttu-id="b4553-135">Дополнительные сведения о жизненном цикле назначения.</span><span class="sxs-lookup"><span data-stu-id="b4553-135">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="b4553-136">Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="b4553-136">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="b4553-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-137">Read-only.</span></span>|
|<span data-ttu-id="b4553-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="b4553-138">catalogId</span></span>|<span data-ttu-id="b4553-139">String</span><span class="sxs-lookup"><span data-stu-id="b4553-139">String</span></span>|<span data-ttu-id="b4553-140">Идентификатор каталога, содержащего пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-140">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="b4553-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-141">Read-only.</span></span>|
|<span data-ttu-id="b4553-142">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="b4553-142">expiredDateTime</span></span>|<span data-ttu-id="b4553-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4553-143">DateTimeOffset</span></span>|<span data-ttu-id="b4553-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b4553-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4553-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b4553-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b4553-146">id</span><span class="sxs-lookup"><span data-stu-id="b4553-146">id</span></span>|<span data-ttu-id="b4553-147">String</span><span class="sxs-lookup"><span data-stu-id="b4553-147">String</span></span>| <span data-ttu-id="b4553-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-148">Read-only.</span></span>|
|<span data-ttu-id="b4553-149">isExtended</span><span class="sxs-lookup"><span data-stu-id="b4553-149">isExtended</span></span>|<span data-ttu-id="b4553-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4553-150">Boolean</span></span>|<span data-ttu-id="b4553-151">Указывает, расширено ли назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-151">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="b4553-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-152">Read-only.</span></span>|
|<span data-ttu-id="b4553-153">targetId</span><span class="sxs-lookup"><span data-stu-id="b4553-153">targetId</span></span>|<span data-ttu-id="b4553-154">String</span><span class="sxs-lookup"><span data-stu-id="b4553-154">String</span></span>| <span data-ttu-id="b4553-155">ID субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="b4553-155">The ID of the subject with the assignment.</span></span> <span data-ttu-id="b4553-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-156">Read-only.</span></span>|
|<span data-ttu-id="b4553-157">schedule</span><span class="sxs-lookup"><span data-stu-id="b4553-157">schedule</span></span>|[<span data-ttu-id="b4553-158">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="b4553-158">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="b4553-159">Когда назначение доступа должно быть на месте.</span><span class="sxs-lookup"><span data-stu-id="b4553-159">When the access assignment is to be in place.</span></span> <span data-ttu-id="b4553-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-160">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4553-161">Связи</span><span class="sxs-lookup"><span data-stu-id="b4553-161">Relationships</span></span>

| <span data-ttu-id="b4553-162">Связь</span><span class="sxs-lookup"><span data-stu-id="b4553-162">Relationship</span></span> | <span data-ttu-id="b4553-163">Тип</span><span class="sxs-lookup"><span data-stu-id="b4553-163">Type</span></span>        | <span data-ttu-id="b4553-164">Описание</span><span class="sxs-lookup"><span data-stu-id="b4553-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4553-165">accessPackage</span><span class="sxs-lookup"><span data-stu-id="b4553-165">accessPackage</span></span>|[<span data-ttu-id="b4553-166">accessPackage</span><span class="sxs-lookup"><span data-stu-id="b4553-166">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="b4553-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-167">Read-only.</span></span> <span data-ttu-id="b4553-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b4553-168">Nullable.</span></span>|
|<span data-ttu-id="b4553-169">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="b4553-169">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="b4553-170">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="b4553-170">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="b4553-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-171">Read-only.</span></span> <span data-ttu-id="b4553-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b4553-172">Nullable.</span></span>|
|<span data-ttu-id="b4553-173">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="b4553-173">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="b4553-174">[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="b4553-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="b4553-175">Роли ресурсов, переданные целевому пользователю для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="b4553-175">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="b4553-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-176">Read-only.</span></span> <span data-ttu-id="b4553-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b4553-177">Nullable.</span></span>|
|<span data-ttu-id="b4553-178">target</span><span class="sxs-lookup"><span data-stu-id="b4553-178">target</span></span>|[<span data-ttu-id="b4553-179">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="b4553-179">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="b4553-180">Тема назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b4553-180">The subject of the access package assignment.</span></span> <span data-ttu-id="b4553-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4553-181">Read-only.</span></span> <span data-ttu-id="b4553-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b4553-182">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4553-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4553-183">JSON representation</span></span>

<span data-ttu-id="b4553-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4553-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


