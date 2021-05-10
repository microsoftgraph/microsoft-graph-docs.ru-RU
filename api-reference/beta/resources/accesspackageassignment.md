---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd352fe67c3afabb1819ffc58d7081dbdae1525c
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298514"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="a6179-103">тип ресурса accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="a6179-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="a6179-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6179-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6179-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="a6179-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="a6179-106">Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6179-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="a6179-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a6179-107">Methods</span></span>

| <span data-ttu-id="a6179-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a6179-108">Method</span></span>       | <span data-ttu-id="a6179-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6179-109">Return Type</span></span> | <span data-ttu-id="a6179-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6179-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a6179-111">Списки accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="a6179-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="a6179-112">[коллекция accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a6179-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="a6179-113">Извлечение списка **объектов accessPackageAssignment.**</span><span class="sxs-lookup"><span data-stu-id="a6179-113">Retrieve a list of **accessPackageAssignment** objects.</span></span> |
|[<span data-ttu-id="a6179-114">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="a6179-114">filterByCurrentUser</span></span>](../api/accesspackageassignment-filterbycurrentuser.md)|<span data-ttu-id="a6179-115">[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a6179-115">[accessPackageAssignment](../resources/accesspackageassignment.md) collection</span></span>|<span data-ttu-id="a6179-116">Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6179-116">Retrieve the list of **accessPackageAssignment** objects filtered on the signed-in user.</span></span>|

><span data-ttu-id="a6179-117">**Примечание:** Вы не можете использовать метод для создания или удаления назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-117">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="a6179-118">Вместо этого клиент, который хочет запросить назначение пакета доступа для пользователя или удалить назначение пакета доступа у пользователя, может создать [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="a6179-118">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6179-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6179-119">Properties</span></span>

| <span data-ttu-id="a6179-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6179-120">Property</span></span>     | <span data-ttu-id="a6179-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a6179-121">Type</span></span>        | <span data-ttu-id="a6179-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a6179-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6179-123">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="a6179-123">accessPackageId</span></span>|<span data-ttu-id="a6179-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-124">String</span></span>|<span data-ttu-id="a6179-125">Идентификатор пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-125">The identifier of the access package.</span></span> <span data-ttu-id="a6179-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-126">Read-only.</span></span>|
|<span data-ttu-id="a6179-127">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="a6179-127">assignmentPolicyId</span></span>|<span data-ttu-id="a6179-128">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-128">String</span></span>|<span data-ttu-id="a6179-129">Идентификатор политики назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-129">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="a6179-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-130">Read-only.</span></span>|
|<span data-ttu-id="a6179-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a6179-131">assignmentState</span></span>|<span data-ttu-id="a6179-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-132">String</span></span>|<span data-ttu-id="a6179-133">Состояние назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-133">The state of the access package assignment.</span></span> <span data-ttu-id="a6179-134">Возможные значения `Delivering` , `Delivered` или `Expired` .</span><span class="sxs-lookup"><span data-stu-id="a6179-134">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="a6179-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-135">Read-only.</span></span>|
|<span data-ttu-id="a6179-136">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="a6179-136">assignmentStatus</span></span>|<span data-ttu-id="a6179-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-137">String</span></span>|<span data-ttu-id="a6179-138">Дополнительные сведения о жизненном цикле назначения.</span><span class="sxs-lookup"><span data-stu-id="a6179-138">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="a6179-139">Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="a6179-139">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="a6179-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-140">Read-only.</span></span>|
|<span data-ttu-id="a6179-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="a6179-141">catalogId</span></span>|<span data-ttu-id="a6179-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-142">String</span></span>|<span data-ttu-id="a6179-143">Идентификатор каталога, содержащего пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-143">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="a6179-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-144">Read-only.</span></span>|
|<span data-ttu-id="a6179-145">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="a6179-145">expiredDateTime</span></span>|<span data-ttu-id="a6179-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6179-146">DateTimeOffset</span></span>|<span data-ttu-id="a6179-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a6179-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6179-148">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a6179-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a6179-149">id</span><span class="sxs-lookup"><span data-stu-id="a6179-149">id</span></span>|<span data-ttu-id="a6179-150">String</span><span class="sxs-lookup"><span data-stu-id="a6179-150">String</span></span>| <span data-ttu-id="a6179-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-151">Read-only.</span></span>|
|<span data-ttu-id="a6179-152">isExtended</span><span class="sxs-lookup"><span data-stu-id="a6179-152">isExtended</span></span>|<span data-ttu-id="a6179-153">Логический</span><span class="sxs-lookup"><span data-stu-id="a6179-153">Boolean</span></span>|<span data-ttu-id="a6179-154">Указывает, расширено ли назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-154">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="a6179-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-155">Read-only.</span></span>|
|<span data-ttu-id="a6179-156">targetId</span><span class="sxs-lookup"><span data-stu-id="a6179-156">targetId</span></span>|<span data-ttu-id="a6179-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a6179-157">String</span></span>| <span data-ttu-id="a6179-158">ID субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="a6179-158">The ID of the subject with the assignment.</span></span> <span data-ttu-id="a6179-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-159">Read-only.</span></span>|
|<span data-ttu-id="a6179-160">schedule</span><span class="sxs-lookup"><span data-stu-id="a6179-160">schedule</span></span>|[<span data-ttu-id="a6179-161">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="a6179-161">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="a6179-162">Когда назначение доступа должно быть на месте.</span><span class="sxs-lookup"><span data-stu-id="a6179-162">When the access assignment is to be in place.</span></span> <span data-ttu-id="a6179-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-163">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6179-164">Связи</span><span class="sxs-lookup"><span data-stu-id="a6179-164">Relationships</span></span>

| <span data-ttu-id="a6179-165">Связь</span><span class="sxs-lookup"><span data-stu-id="a6179-165">Relationship</span></span> | <span data-ttu-id="a6179-166">Тип</span><span class="sxs-lookup"><span data-stu-id="a6179-166">Type</span></span>        | <span data-ttu-id="a6179-167">Описание</span><span class="sxs-lookup"><span data-stu-id="a6179-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6179-168">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6179-168">accessPackage</span></span>|[<span data-ttu-id="a6179-169">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6179-169">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="a6179-p112">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6179-p112">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a6179-172">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="a6179-172">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="a6179-173">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="a6179-173">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="a6179-p113">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6179-p113">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a6179-176">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="a6179-176">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="a6179-177">[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="a6179-177">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="a6179-178">Роли ресурсов, переданные целевому пользователю для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="a6179-178">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="a6179-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-179">Read-only.</span></span> <span data-ttu-id="a6179-180">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6179-180">Nullable.</span></span>|
|<span data-ttu-id="a6179-181">target</span><span class="sxs-lookup"><span data-stu-id="a6179-181">target</span></span>|[<span data-ttu-id="a6179-182">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="a6179-182">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="a6179-183">Тема назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a6179-183">The subject of the access package assignment.</span></span> <span data-ttu-id="a6179-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6179-184">Read-only.</span></span> <span data-ttu-id="a6179-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a6179-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6179-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6179-186">JSON representation</span></span>

<span data-ttu-id="a6179-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6179-187">The following is a JSON representation of the resource.</span></span>

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


