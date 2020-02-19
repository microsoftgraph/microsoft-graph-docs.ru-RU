---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7147378e308faac7ca1fea931a465e1ea54f22ef
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108450"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="ec8f5-103">Тип ресурса Акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="ec8f5-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec8f5-104">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="ec8f5-105">Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="ec8f5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ec8f5-106">Methods</span></span>

| <span data-ttu-id="ec8f5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ec8f5-107">Method</span></span>       | <span data-ttu-id="ec8f5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec8f5-108">Return Type</span></span> | <span data-ttu-id="ec8f5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec8f5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ec8f5-110">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="ec8f5-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="ec8f5-111">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec8f5-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="ec8f5-112">Получение списка объектов **акцесспаккажеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="ec8f5-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="ec8f5-113">**Примечание:** Невозможно использовать метод для создания или удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-113">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="ec8f5-114">Вместо этого клиент, которому требуется запрашивать назначение пакета доступа для пользователя или удалять назначение пакета Access пользователю, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="ec8f5-114">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ec8f5-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec8f5-115">Properties</span></span>

| <span data-ttu-id="ec8f5-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec8f5-116">Property</span></span>     | <span data-ttu-id="ec8f5-117">Тип</span><span class="sxs-lookup"><span data-stu-id="ec8f5-117">Type</span></span>        | <span data-ttu-id="ec8f5-118">Описание</span><span class="sxs-lookup"><span data-stu-id="ec8f5-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec8f5-119">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="ec8f5-119">accessPackageId</span></span>|<span data-ttu-id="ec8f5-120">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-120">String</span></span>|<span data-ttu-id="ec8f5-121">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-121">The identifier of the access package.</span></span> <span data-ttu-id="ec8f5-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-122">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-123">ассигнментполициид</span><span class="sxs-lookup"><span data-stu-id="ec8f5-123">assignmentPolicyId</span></span>|<span data-ttu-id="ec8f5-124">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-124">String</span></span>|<span data-ttu-id="ec8f5-125">Идентификатор политики назначения пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="ec8f5-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-126">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-127">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="ec8f5-127">assignmentState</span></span>|<span data-ttu-id="ec8f5-128">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-128">String</span></span>|<span data-ttu-id="ec8f5-129">Состояние пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-129">The state of the access package.</span></span> <span data-ttu-id="ec8f5-130">Возможные значения: `Delivered` или `Expired`.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-130">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="ec8f5-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-131">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-132">Свойства assignmentstatus</span><span class="sxs-lookup"><span data-stu-id="ec8f5-132">assignmentStatus</span></span>|<span data-ttu-id="ec8f5-133">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-133">String</span></span>|<span data-ttu-id="ec8f5-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-134">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-135">каталогид</span><span class="sxs-lookup"><span data-stu-id="ec8f5-135">catalogId</span></span>|<span data-ttu-id="ec8f5-136">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-136">String</span></span>|<span data-ttu-id="ec8f5-137">Идентификатор каталога, содержащего пакет Access.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-137">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="ec8f5-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-138">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-139">експиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="ec8f5-139">expiredDateTime</span></span>|<span data-ttu-id="ec8f5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8f5-140">DateTimeOffset</span></span>|<span data-ttu-id="ec8f5-p107">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ec8f5-143">id</span><span class="sxs-lookup"><span data-stu-id="ec8f5-143">id</span></span>|<span data-ttu-id="ec8f5-144">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-144">String</span></span>| <span data-ttu-id="ec8f5-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-145">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-146">Расширенная</span><span class="sxs-lookup"><span data-stu-id="ec8f5-146">isExtended</span></span>|<span data-ttu-id="ec8f5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec8f5-147">Boolean</span></span>|<span data-ttu-id="ec8f5-148">Указывает, является ли назначение пакета доступа расширенным.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-148">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="ec8f5-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-149">Read-only.</span></span>|
|<span data-ttu-id="ec8f5-150">targetId</span><span class="sxs-lookup"><span data-stu-id="ec8f5-150">targetId</span></span>|<span data-ttu-id="ec8f5-151">String</span><span class="sxs-lookup"><span data-stu-id="ec8f5-151">String</span></span>| <span data-ttu-id="ec8f5-152">ИДЕНТИФИКАТОР субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-152">The ID of the subject with the assignment.</span></span> <span data-ttu-id="ec8f5-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec8f5-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="ec8f5-154">Relationships</span></span>

| <span data-ttu-id="ec8f5-155">Связь</span><span class="sxs-lookup"><span data-stu-id="ec8f5-155">Relationship</span></span> | <span data-ttu-id="ec8f5-156">Тип</span><span class="sxs-lookup"><span data-stu-id="ec8f5-156">Type</span></span>        | <span data-ttu-id="ec8f5-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ec8f5-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec8f5-158">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="ec8f5-158">accessPackage</span></span>|[<span data-ttu-id="ec8f5-159">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="ec8f5-159">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="ec8f5-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-160">Read-only.</span></span> <span data-ttu-id="ec8f5-161">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-161">Nullable.</span></span>|
|<span data-ttu-id="ec8f5-162">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="ec8f5-162">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="ec8f5-163">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="ec8f5-163">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="ec8f5-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-164">Read-only.</span></span> <span data-ttu-id="ec8f5-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-165">Nullable.</span></span>|
|<span data-ttu-id="ec8f5-166">акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="ec8f5-166">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="ec8f5-167">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="ec8f5-167">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="ec8f5-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-168">Read-only.</span></span> <span data-ttu-id="ec8f5-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-169">Nullable.</span></span>|
|<span data-ttu-id="ec8f5-170">target</span><span class="sxs-lookup"><span data-stu-id="ec8f5-170">target</span></span>|[<span data-ttu-id="ec8f5-171">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="ec8f5-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ec8f5-172">Тема назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-172">The subject of the access package assignment.</span></span> <span data-ttu-id="ec8f5-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-173">Read-only.</span></span> <span data-ttu-id="ec8f5-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec8f5-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec8f5-175">JSON representation</span></span>

<span data-ttu-id="ec8f5-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec8f5-176">The following is a JSON representation of the resource.</span></span>

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
            "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
            "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
            "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
            "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
            "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
            "assignmentStatus": "ExpiredNotificationTriggered",
            "assignmentState": "Expired",
            "isExtended": false,
            "expiredDateTime": "2019-04-25T23:45:40.42Z"
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
