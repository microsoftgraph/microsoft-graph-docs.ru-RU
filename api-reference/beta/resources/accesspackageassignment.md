---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f7a2fe772dc7b3be328fad452a5b193ccf7a7ed0
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319460"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="f2901-103">Тип ресурса Акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="f2901-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="f2901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2901-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2901-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="f2901-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="f2901-106">Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.</span><span class="sxs-lookup"><span data-stu-id="f2901-106">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="f2901-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f2901-107">Methods</span></span>

| <span data-ttu-id="f2901-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f2901-108">Method</span></span>       | <span data-ttu-id="f2901-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2901-109">Return Type</span></span> | <span data-ttu-id="f2901-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2901-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f2901-111">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="f2901-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="f2901-112">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f2901-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="f2901-113">Получение списка объектов **акцесспаккажеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="f2901-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="f2901-114">**Примечание:** Невозможно использовать метод для создания или удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="f2901-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="f2901-115">Вместо этого клиент, которому требуется запрашивать назначение пакета доступа для пользователя или удалять назначение пакета Access пользователю, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="f2901-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f2901-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2901-116">Properties</span></span>

| <span data-ttu-id="f2901-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2901-117">Property</span></span>     | <span data-ttu-id="f2901-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f2901-118">Type</span></span>        | <span data-ttu-id="f2901-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f2901-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2901-120">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="f2901-120">accessPackageId</span></span>|<span data-ttu-id="f2901-121">String</span><span class="sxs-lookup"><span data-stu-id="f2901-121">String</span></span>|<span data-ttu-id="f2901-122">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="f2901-122">The identifier of the access package.</span></span> <span data-ttu-id="f2901-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-123">Read-only.</span></span>|
|<span data-ttu-id="f2901-124">ассигнментполициид</span><span class="sxs-lookup"><span data-stu-id="f2901-124">assignmentPolicyId</span></span>|<span data-ttu-id="f2901-125">String</span><span class="sxs-lookup"><span data-stu-id="f2901-125">String</span></span>|<span data-ttu-id="f2901-126">Идентификатор политики назначения пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="f2901-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="f2901-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-127">Read-only.</span></span>|
|<span data-ttu-id="f2901-128">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f2901-128">assignmentState</span></span>|<span data-ttu-id="f2901-129">String</span><span class="sxs-lookup"><span data-stu-id="f2901-129">String</span></span>|<span data-ttu-id="f2901-130">Состояние пакета Access.</span><span class="sxs-lookup"><span data-stu-id="f2901-130">The state of the access package.</span></span> <span data-ttu-id="f2901-131">Возможные значения: `Delivered` или `Expired` .</span><span class="sxs-lookup"><span data-stu-id="f2901-131">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="f2901-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-132">Read-only.</span></span>|
|<span data-ttu-id="f2901-133">Свойства assignmentstatus</span><span class="sxs-lookup"><span data-stu-id="f2901-133">assignmentStatus</span></span>|<span data-ttu-id="f2901-134">String</span><span class="sxs-lookup"><span data-stu-id="f2901-134">String</span></span>|<span data-ttu-id="f2901-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-135">Read-only.</span></span>|
|<span data-ttu-id="f2901-136">каталогид</span><span class="sxs-lookup"><span data-stu-id="f2901-136">catalogId</span></span>|<span data-ttu-id="f2901-137">String</span><span class="sxs-lookup"><span data-stu-id="f2901-137">String</span></span>|<span data-ttu-id="f2901-138">Идентификатор каталога, содержащего пакет Access.</span><span class="sxs-lookup"><span data-stu-id="f2901-138">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="f2901-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-139">Read-only.</span></span>|
|<span data-ttu-id="f2901-140">експиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="f2901-140">expiredDateTime</span></span>|<span data-ttu-id="f2901-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2901-141">DateTimeOffset</span></span>|<span data-ttu-id="f2901-p107">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f2901-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2901-144">id</span><span class="sxs-lookup"><span data-stu-id="f2901-144">id</span></span>|<span data-ttu-id="f2901-145">String</span><span class="sxs-lookup"><span data-stu-id="f2901-145">String</span></span>| <span data-ttu-id="f2901-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-146">Read-only.</span></span>|
|<span data-ttu-id="f2901-147">Расширенная</span><span class="sxs-lookup"><span data-stu-id="f2901-147">isExtended</span></span>|<span data-ttu-id="f2901-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2901-148">Boolean</span></span>|<span data-ttu-id="f2901-149">Указывает, является ли назначение пакета доступа расширенным.</span><span class="sxs-lookup"><span data-stu-id="f2901-149">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="f2901-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-150">Read-only.</span></span>|
|<span data-ttu-id="f2901-151">targetId</span><span class="sxs-lookup"><span data-stu-id="f2901-151">targetId</span></span>|<span data-ttu-id="f2901-152">String</span><span class="sxs-lookup"><span data-stu-id="f2901-152">String</span></span>| <span data-ttu-id="f2901-153">ИДЕНТИФИКАТОР субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="f2901-153">The ID of the subject with the assignment.</span></span> <span data-ttu-id="f2901-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2901-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="f2901-155">Relationships</span></span>

| <span data-ttu-id="f2901-156">Связь</span><span class="sxs-lookup"><span data-stu-id="f2901-156">Relationship</span></span> | <span data-ttu-id="f2901-157">Тип</span><span class="sxs-lookup"><span data-stu-id="f2901-157">Type</span></span>        | <span data-ttu-id="f2901-158">Описание</span><span class="sxs-lookup"><span data-stu-id="f2901-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2901-159">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="f2901-159">accessPackage</span></span>|[<span data-ttu-id="f2901-160">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="f2901-160">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="f2901-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-161">Read-only.</span></span> <span data-ttu-id="f2901-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f2901-162">Nullable.</span></span>|
|<span data-ttu-id="f2901-163">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="f2901-163">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="f2901-164">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="f2901-164">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="f2901-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-165">Read-only.</span></span> <span data-ttu-id="f2901-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f2901-166">Nullable.</span></span>|
|<span data-ttu-id="f2901-167">акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="f2901-167">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="f2901-168">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="f2901-168">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="f2901-169">Роли ресурсов, доставляемые конечному пользователю для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="f2901-169">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="f2901-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-170">Read-only.</span></span> <span data-ttu-id="f2901-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f2901-171">Nullable.</span></span>|
|<span data-ttu-id="f2901-172">target</span><span class="sxs-lookup"><span data-stu-id="f2901-172">target</span></span>|[<span data-ttu-id="f2901-173">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="f2901-173">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="f2901-174">Тема назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="f2901-174">The subject of the access package assignment.</span></span> <span data-ttu-id="f2901-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2901-175">Read-only.</span></span> <span data-ttu-id="f2901-176">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f2901-176">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2901-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2901-177">JSON representation</span></span>

<span data-ttu-id="f2901-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2901-178">The following is a JSON representation of the resource.</span></span>

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
