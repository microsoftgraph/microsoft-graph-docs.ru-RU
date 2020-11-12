---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd85461a4429801aad5145256c711278789c95ed
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000709"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="9b027-103">Тип ресурса Акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="9b027-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="9b027-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b027-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b027-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="9b027-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="9b027-106">Например, при назначении пакета доступа может быть задано, что пользователю Алиса был назначен доступ через пакет доступа Sales за период с 2019 по 2019 июля.</span><span class="sxs-lookup"><span data-stu-id="9b027-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="9b027-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9b027-107">Methods</span></span>

| <span data-ttu-id="9b027-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9b027-108">Method</span></span>       | <span data-ttu-id="9b027-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b027-109">Return Type</span></span> | <span data-ttu-id="9b027-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b027-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9b027-111">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="9b027-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="9b027-112">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b027-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="9b027-113">Получение списка объектов **акцесспаккажеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="9b027-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="9b027-114">**Примечание:** Невозможно использовать метод для создания или удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9b027-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="9b027-115">Вместо этого клиент, которому требуется запрашивать назначение пакета доступа для пользователя или удалять назначение пакета Access пользователю, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="9b027-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9b027-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b027-116">Properties</span></span>

| <span data-ttu-id="9b027-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b027-117">Property</span></span>     | <span data-ttu-id="9b027-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9b027-118">Type</span></span>        | <span data-ttu-id="9b027-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9b027-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b027-120">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="9b027-120">accessPackageId</span></span>|<span data-ttu-id="9b027-121">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-121">String</span></span>|<span data-ttu-id="9b027-122">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9b027-122">The identifier of the access package.</span></span> <span data-ttu-id="9b027-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-123">Read-only.</span></span>|
|<span data-ttu-id="9b027-124">ассигнментполициид</span><span class="sxs-lookup"><span data-stu-id="9b027-124">assignmentPolicyId</span></span>|<span data-ttu-id="9b027-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-125">String</span></span>|<span data-ttu-id="9b027-126">Идентификатор политики назначения пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="9b027-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="9b027-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-127">Read-only.</span></span>|
|<span data-ttu-id="9b027-128">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="9b027-128">assignmentState</span></span>|<span data-ttu-id="9b027-129">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-129">String</span></span>|<span data-ttu-id="9b027-130">Состояние назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9b027-130">The state of the access package assignment.</span></span> <span data-ttu-id="9b027-131">Возможные значения: `Delivering` , `Delivered` , или `Expired` .</span><span class="sxs-lookup"><span data-stu-id="9b027-131">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="9b027-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-132">Read-only.</span></span>|
|<span data-ttu-id="9b027-133">Свойства assignmentstatus</span><span class="sxs-lookup"><span data-stu-id="9b027-133">assignmentStatus</span></span>|<span data-ttu-id="9b027-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-134">String</span></span>|<span data-ttu-id="9b027-135">Дополнительные сведения о жизненном цикле назначения.</span><span class="sxs-lookup"><span data-stu-id="9b027-135">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="9b027-136">Возможные значения: `Delivering` , `Delivered` , `NearExpiry1DayNotificationTriggered` , или `ExpiredNotificationTriggered` .</span><span class="sxs-lookup"><span data-stu-id="9b027-136">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="9b027-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-137">Read-only.</span></span>|
|<span data-ttu-id="9b027-138">каталогид</span><span class="sxs-lookup"><span data-stu-id="9b027-138">catalogId</span></span>|<span data-ttu-id="9b027-139">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-139">String</span></span>|<span data-ttu-id="9b027-140">Идентификатор каталога, содержащего пакет Access.</span><span class="sxs-lookup"><span data-stu-id="9b027-140">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="9b027-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-141">Read-only.</span></span>|
|<span data-ttu-id="9b027-142">експиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="9b027-142">expiredDateTime</span></span>|<span data-ttu-id="9b027-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b027-143">DateTimeOffset</span></span>|<span data-ttu-id="9b027-p108">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9b027-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b027-146">id</span><span class="sxs-lookup"><span data-stu-id="9b027-146">id</span></span>|<span data-ttu-id="9b027-147">String</span><span class="sxs-lookup"><span data-stu-id="9b027-147">String</span></span>| <span data-ttu-id="9b027-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-148">Read-only.</span></span>|
|<span data-ttu-id="9b027-149">Расширенная</span><span class="sxs-lookup"><span data-stu-id="9b027-149">isExtended</span></span>|<span data-ttu-id="9b027-150">Логический</span><span class="sxs-lookup"><span data-stu-id="9b027-150">Boolean</span></span>|<span data-ttu-id="9b027-151">Указывает, является ли назначение пакета доступа расширенным.</span><span class="sxs-lookup"><span data-stu-id="9b027-151">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="9b027-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-152">Read-only.</span></span>|
|<span data-ttu-id="9b027-153">targetId</span><span class="sxs-lookup"><span data-stu-id="9b027-153">targetId</span></span>|<span data-ttu-id="9b027-154">Строка</span><span class="sxs-lookup"><span data-stu-id="9b027-154">String</span></span>| <span data-ttu-id="9b027-155">ИДЕНТИФИКАТОР субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="9b027-155">The ID of the subject with the assignment.</span></span> <span data-ttu-id="9b027-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-156">Read-only.</span></span>|
|<span data-ttu-id="9b027-157">schedule</span><span class="sxs-lookup"><span data-stu-id="9b027-157">schedule</span></span>|[<span data-ttu-id="9b027-158">рекуестсчедуле</span><span class="sxs-lookup"><span data-stu-id="9b027-158">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="9b027-159">Когда назначение доступа будет размещено.</span><span class="sxs-lookup"><span data-stu-id="9b027-159">When the access assignment is to be in place.</span></span> <span data-ttu-id="9b027-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-160">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b027-161">Связи</span><span class="sxs-lookup"><span data-stu-id="9b027-161">Relationships</span></span>

| <span data-ttu-id="9b027-162">Связь</span><span class="sxs-lookup"><span data-stu-id="9b027-162">Relationship</span></span> | <span data-ttu-id="9b027-163">Тип</span><span class="sxs-lookup"><span data-stu-id="9b027-163">Type</span></span>        | <span data-ttu-id="9b027-164">Описание</span><span class="sxs-lookup"><span data-stu-id="9b027-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b027-165">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="9b027-165">accessPackage</span></span>|[<span data-ttu-id="9b027-166">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="9b027-166">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="9b027-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-167">Read-only.</span></span> <span data-ttu-id="9b027-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b027-168">Nullable.</span></span>|
|<span data-ttu-id="9b027-169">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9b027-169">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="9b027-170">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9b027-170">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="9b027-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-171">Read-only.</span></span> <span data-ttu-id="9b027-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b027-172">Nullable.</span></span>|
|<span data-ttu-id="9b027-173">акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="9b027-173">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="9b027-174">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9b027-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="9b027-175">Роли ресурсов, доставляемые конечному пользователю для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="9b027-175">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="9b027-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-176">Read-only.</span></span> <span data-ttu-id="9b027-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b027-177">Nullable.</span></span>|
|<span data-ttu-id="9b027-178">target</span><span class="sxs-lookup"><span data-stu-id="9b027-178">target</span></span>|[<span data-ttu-id="9b027-179">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="9b027-179">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="9b027-180">Тема назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9b027-180">The subject of the access package assignment.</span></span> <span data-ttu-id="9b027-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b027-181">Read-only.</span></span> <span data-ttu-id="9b027-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b027-182">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b027-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b027-183">JSON representation</span></span>

<span data-ttu-id="9b027-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b027-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "",
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


