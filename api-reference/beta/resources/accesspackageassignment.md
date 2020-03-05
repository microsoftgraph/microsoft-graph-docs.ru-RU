---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b52b9dbd7b2b76df34ab6c55a46b69718d4a0e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508564"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="2b6d5-103">Тип ресурса Акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2b6d5-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="2b6d5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b6d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b6d5-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="2b6d5-106">Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-106">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="2b6d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2b6d5-107">Methods</span></span>

| <span data-ttu-id="2b6d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2b6d5-108">Method</span></span>       | <span data-ttu-id="2b6d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b6d5-109">Return Type</span></span> | <span data-ttu-id="2b6d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6d5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2b6d5-111">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="2b6d5-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="2b6d5-112">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2b6d5-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="2b6d5-113">Получение списка объектов **акцесспаккажеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="2b6d5-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="2b6d5-114">**Примечание:** Невозможно использовать метод для создания или удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="2b6d5-115">Вместо этого клиент, которому требуется запрашивать назначение пакета доступа для пользователя или удалять назначение пакета Access пользователю, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="2b6d5-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2b6d5-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b6d5-116">Properties</span></span>

| <span data-ttu-id="2b6d5-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b6d5-117">Property</span></span>     | <span data-ttu-id="2b6d5-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2b6d5-118">Type</span></span>        | <span data-ttu-id="2b6d5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6d5-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b6d5-120">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="2b6d5-120">accessPackageId</span></span>|<span data-ttu-id="2b6d5-121">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-121">String</span></span>|<span data-ttu-id="2b6d5-122">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-122">The identifier of the access package.</span></span> <span data-ttu-id="2b6d5-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-123">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-124">ассигнментполициид</span><span class="sxs-lookup"><span data-stu-id="2b6d5-124">assignmentPolicyId</span></span>|<span data-ttu-id="2b6d5-125">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-125">String</span></span>|<span data-ttu-id="2b6d5-126">Идентификатор политики назначения пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="2b6d5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-127">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-128">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2b6d5-128">assignmentState</span></span>|<span data-ttu-id="2b6d5-129">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-129">String</span></span>|<span data-ttu-id="2b6d5-130">Состояние пакета Access.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-130">The state of the access package.</span></span> <span data-ttu-id="2b6d5-131">Возможные значения: `Delivered` или `Expired`.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-131">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="2b6d5-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-132">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-133">Свойства assignmentstatus</span><span class="sxs-lookup"><span data-stu-id="2b6d5-133">assignmentStatus</span></span>|<span data-ttu-id="2b6d5-134">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-134">String</span></span>|<span data-ttu-id="2b6d5-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-135">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-136">каталогид</span><span class="sxs-lookup"><span data-stu-id="2b6d5-136">catalogId</span></span>|<span data-ttu-id="2b6d5-137">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-137">String</span></span>|<span data-ttu-id="2b6d5-138">Идентификатор каталога, содержащего пакет Access.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-138">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="2b6d5-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-139">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-140">експиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="2b6d5-140">expiredDateTime</span></span>|<span data-ttu-id="2b6d5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6d5-141">DateTimeOffset</span></span>|<span data-ttu-id="2b6d5-p107">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2b6d5-144">id</span><span class="sxs-lookup"><span data-stu-id="2b6d5-144">id</span></span>|<span data-ttu-id="2b6d5-145">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-145">String</span></span>| <span data-ttu-id="2b6d5-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-146">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-147">Расширенная</span><span class="sxs-lookup"><span data-stu-id="2b6d5-147">isExtended</span></span>|<span data-ttu-id="2b6d5-148">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6d5-148">Boolean</span></span>|<span data-ttu-id="2b6d5-149">Указывает, является ли назначение пакета доступа расширенным.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-149">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="2b6d5-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-150">Read-only.</span></span>|
|<span data-ttu-id="2b6d5-151">targetId</span><span class="sxs-lookup"><span data-stu-id="2b6d5-151">targetId</span></span>|<span data-ttu-id="2b6d5-152">String</span><span class="sxs-lookup"><span data-stu-id="2b6d5-152">String</span></span>| <span data-ttu-id="2b6d5-153">ИДЕНТИФИКАТОР субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-153">The ID of the subject with the assignment.</span></span> <span data-ttu-id="2b6d5-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b6d5-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b6d5-155">Relationships</span></span>

| <span data-ttu-id="2b6d5-156">Связь</span><span class="sxs-lookup"><span data-stu-id="2b6d5-156">Relationship</span></span> | <span data-ttu-id="2b6d5-157">Тип</span><span class="sxs-lookup"><span data-stu-id="2b6d5-157">Type</span></span>        | <span data-ttu-id="2b6d5-158">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6d5-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b6d5-159">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="2b6d5-159">accessPackage</span></span>|[<span data-ttu-id="2b6d5-160">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="2b6d5-160">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="2b6d5-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-161">Read-only.</span></span> <span data-ttu-id="2b6d5-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-162">Nullable.</span></span>|
|<span data-ttu-id="2b6d5-163">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="2b6d5-163">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="2b6d5-164">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="2b6d5-164">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="2b6d5-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-165">Read-only.</span></span> <span data-ttu-id="2b6d5-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-166">Nullable.</span></span>|
|<span data-ttu-id="2b6d5-167">акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="2b6d5-167">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="2b6d5-168">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="2b6d5-168">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="2b6d5-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-169">Read-only.</span></span> <span data-ttu-id="2b6d5-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-170">Nullable.</span></span>|
|<span data-ttu-id="2b6d5-171">target</span><span class="sxs-lookup"><span data-stu-id="2b6d5-171">target</span></span>|[<span data-ttu-id="2b6d5-172">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="2b6d5-172">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="2b6d5-173">Тема назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-173">The subject of the access package assignment.</span></span> <span data-ttu-id="2b6d5-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-174">Read-only.</span></span> <span data-ttu-id="2b6d5-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-175">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b6d5-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b6d5-176">JSON representation</span></span>

<span data-ttu-id="2b6d5-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b6d5-177">The following is a JSON representation of the resource.</span></span>

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
