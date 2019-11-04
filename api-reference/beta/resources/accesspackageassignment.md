---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 234aad48e11a2b6c5c2a47c494216fa15fbc139b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939217"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="27c8c-103">Тип ресурса Акцесспаккажеассигнмент</span><span class="sxs-lookup"><span data-stu-id="27c8c-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27c8c-104">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="27c8c-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="27c8c-105">Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.</span><span class="sxs-lookup"><span data-stu-id="27c8c-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="27c8c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="27c8c-106">Methods</span></span>

| <span data-ttu-id="27c8c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="27c8c-107">Method</span></span>       | <span data-ttu-id="27c8c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27c8c-108">Return Type</span></span> | <span data-ttu-id="27c8c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27c8c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="27c8c-110">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="27c8c-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="27c8c-111">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="27c8c-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="27c8c-112">Получение списка объектов **акцесспаккажеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="27c8c-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="27c8c-113">**Примечание:** Невозможно использовать метод для создания назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="27c8c-113">**Note:** You can't use a method to create an access package assignment.</span></span> <span data-ttu-id="27c8c-114">Вместо этого клиент, которому требуется запросить назначение пакета доступа для пользователя, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="27c8c-114">Instead, a client that wants to request an access package assignment for a user can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="27c8c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="27c8c-115">Properties</span></span>

| <span data-ttu-id="27c8c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="27c8c-116">Property</span></span>     | <span data-ttu-id="27c8c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="27c8c-117">Type</span></span>        | <span data-ttu-id="27c8c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="27c8c-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27c8c-119">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="27c8c-119">accessPackageId</span></span>|<span data-ttu-id="27c8c-120">Строка</span><span class="sxs-lookup"><span data-stu-id="27c8c-120">String</span></span>|<span data-ttu-id="27c8c-121">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="27c8c-121">The identifier of the access package.</span></span> <span data-ttu-id="27c8c-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-122">Read-only.</span></span>|
|<span data-ttu-id="27c8c-123">ассигнментполициид</span><span class="sxs-lookup"><span data-stu-id="27c8c-123">assignmentPolicyId</span></span>|<span data-ttu-id="27c8c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="27c8c-124">String</span></span>|<span data-ttu-id="27c8c-125">Идентификатор политики назначения пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="27c8c-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="27c8c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-126">Read-only.</span></span>|
|<span data-ttu-id="27c8c-127">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="27c8c-127">assignmentState</span></span>|<span data-ttu-id="27c8c-128">String</span><span class="sxs-lookup"><span data-stu-id="27c8c-128">String</span></span>|<span data-ttu-id="27c8c-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-129">Read-only.</span></span>|
|<span data-ttu-id="27c8c-130">Свойства assignmentstatus</span><span class="sxs-lookup"><span data-stu-id="27c8c-130">assignmentStatus</span></span>|<span data-ttu-id="27c8c-131">String</span><span class="sxs-lookup"><span data-stu-id="27c8c-131">String</span></span>|<span data-ttu-id="27c8c-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-132">Read-only.</span></span>|
|<span data-ttu-id="27c8c-133">каталогид</span><span class="sxs-lookup"><span data-stu-id="27c8c-133">catalogId</span></span>|<span data-ttu-id="27c8c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="27c8c-134">String</span></span>|<span data-ttu-id="27c8c-135">Идентификатор каталога, содержащего пакет Access.</span><span class="sxs-lookup"><span data-stu-id="27c8c-135">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="27c8c-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-136">Read-only.</span></span>|
|<span data-ttu-id="27c8c-137">експиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="27c8c-137">expiredDateTime</span></span>|<span data-ttu-id="27c8c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27c8c-138">DateTimeOffset</span></span>|<span data-ttu-id="27c8c-p106">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="27c8c-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="27c8c-141">id</span><span class="sxs-lookup"><span data-stu-id="27c8c-141">id</span></span>|<span data-ttu-id="27c8c-142">String</span><span class="sxs-lookup"><span data-stu-id="27c8c-142">String</span></span>| <span data-ttu-id="27c8c-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-143">Read-only.</span></span>|
|<span data-ttu-id="27c8c-144">Расширенная</span><span class="sxs-lookup"><span data-stu-id="27c8c-144">isExtended</span></span>|<span data-ttu-id="27c8c-145">Логический</span><span class="sxs-lookup"><span data-stu-id="27c8c-145">Boolean</span></span>|<span data-ttu-id="27c8c-146">Указывает, является ли назначение пакета доступа расширенным.</span><span class="sxs-lookup"><span data-stu-id="27c8c-146">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="27c8c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-147">Read-only.</span></span>|
|<span data-ttu-id="27c8c-148">targetId</span><span class="sxs-lookup"><span data-stu-id="27c8c-148">targetId</span></span>|<span data-ttu-id="27c8c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="27c8c-149">String</span></span>| <span data-ttu-id="27c8c-150">ИДЕНТИФИКАТОР субъекта с назначением.</span><span class="sxs-lookup"><span data-stu-id="27c8c-150">The ID of the subject with the assignment.</span></span> <span data-ttu-id="27c8c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27c8c-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="27c8c-152">Relationships</span></span>

| <span data-ttu-id="27c8c-153">Связь</span><span class="sxs-lookup"><span data-stu-id="27c8c-153">Relationship</span></span> | <span data-ttu-id="27c8c-154">Тип</span><span class="sxs-lookup"><span data-stu-id="27c8c-154">Type</span></span>        | <span data-ttu-id="27c8c-155">Описание</span><span class="sxs-lookup"><span data-stu-id="27c8c-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27c8c-156">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="27c8c-156">accessPackage</span></span>|[<span data-ttu-id="27c8c-157">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="27c8c-157">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="27c8c-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-158">Read-only.</span></span> <span data-ttu-id="27c8c-159">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="27c8c-159">Nullable.</span></span>|
|<span data-ttu-id="27c8c-160">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="27c8c-160">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="27c8c-161">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="27c8c-161">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="27c8c-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-162">Read-only.</span></span> <span data-ttu-id="27c8c-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="27c8c-163">Nullable.</span></span>|
|<span data-ttu-id="27c8c-164">акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="27c8c-164">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="27c8c-165">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="27c8c-165">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="27c8c-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-166">Read-only.</span></span> <span data-ttu-id="27c8c-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="27c8c-167">Nullable.</span></span>|
|<span data-ttu-id="27c8c-168">target</span><span class="sxs-lookup"><span data-stu-id="27c8c-168">target</span></span>|[<span data-ttu-id="27c8c-169">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="27c8c-169">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="27c8c-170">Тема назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="27c8c-170">The subject of the access package assignment.</span></span> <span data-ttu-id="27c8c-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c8c-171">Read-only.</span></span> <span data-ttu-id="27c8c-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="27c8c-172">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27c8c-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27c8c-173">JSON representation</span></span>

<span data-ttu-id="27c8c-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27c8c-174">The following is a JSON representation of the resource.</span></span>

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
