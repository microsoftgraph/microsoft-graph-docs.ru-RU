---
title: Тип ресурса Акцесспаккажеассигнментполици
description: Политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: acb7c7b355d2a03d78cad1127882f272135fc4a2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939210"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="13623-103">Тип ресурса Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13623-104">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="13623-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="13623-105">Пакет Access может иметь не более одного или нескольких политик.</span><span class="sxs-lookup"><span data-stu-id="13623-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="13623-106">При получении запроса от субъекта субъект сравнивается с каждой политикой, чтобы найти политику (если она задана) для этой темы.</span><span class="sxs-lookup"><span data-stu-id="13623-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) for that subject.</span></span> <span data-ttu-id="13623-107">Затем политика определяет, требуется ли утверждение запроса и время назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="13623-107">The policy then determines whether the request requires approval, and the duration of the access package assignment.</span></span>

<span data-ttu-id="13623-108">Чтобы назначить пользователя пакету доступа, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , который ссылается на политику назначения пакетов доступа и пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="13623-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="13623-109">Методы</span><span class="sxs-lookup"><span data-stu-id="13623-109">Methods</span></span>

| <span data-ttu-id="13623-110">Метод</span><span class="sxs-lookup"><span data-stu-id="13623-110">Method</span></span>       | <span data-ttu-id="13623-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13623-111">Return Type</span></span> | <span data-ttu-id="13623-112">Описание</span><span class="sxs-lookup"><span data-stu-id="13623-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13623-113">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="13623-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="13623-114">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="13623-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="13623-115">Получение списка объектов Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="13623-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="13623-116">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="13623-117">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="13623-118">Создание нового объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="13623-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="13623-119">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="13623-120">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="13623-121">Чтение свойств и связей объекта Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="13623-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="13623-122">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="13623-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="13623-123">Удаление Акцесспаккажеассигнментполици.</span><span class="sxs-lookup"><span data-stu-id="13623-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="13623-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="13623-124">Properties</span></span>

| <span data-ttu-id="13623-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="13623-125">Property</span></span>     | <span data-ttu-id="13623-126">Тип</span><span class="sxs-lookup"><span data-stu-id="13623-126">Type</span></span>        | <span data-ttu-id="13623-127">Описание</span><span class="sxs-lookup"><span data-stu-id="13623-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13623-128">акцесспаккажеид</span><span class="sxs-lookup"><span data-stu-id="13623-128">accessPackageId</span></span>|<span data-ttu-id="13623-129">Строка</span><span class="sxs-lookup"><span data-stu-id="13623-129">String</span></span>|<span data-ttu-id="13623-130">Идентификатор пакета Access.</span><span class="sxs-lookup"><span data-stu-id="13623-130">ID of the access package.</span></span>|
|<span data-ttu-id="13623-131">canExtend</span><span class="sxs-lookup"><span data-stu-id="13623-131">canExtend</span></span>|<span data-ttu-id="13623-132">Логический</span><span class="sxs-lookup"><span data-stu-id="13623-132">Boolean</span></span>|<span data-ttu-id="13623-133">Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="13623-133">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="13623-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="13623-134">createdBy</span></span>|<span data-ttu-id="13623-135">String</span><span class="sxs-lookup"><span data-stu-id="13623-135">String</span></span>|<span data-ttu-id="13623-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13623-136">Read-only.</span></span>|
|<span data-ttu-id="13623-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13623-137">createdDateTime</span></span>|<span data-ttu-id="13623-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13623-138">DateTimeOffset</span></span>|<span data-ttu-id="13623-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13623-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="13623-141">description</span><span class="sxs-lookup"><span data-stu-id="13623-141">description</span></span>|<span data-ttu-id="13623-142">String</span><span class="sxs-lookup"><span data-stu-id="13623-142">String</span></span>|<span data-ttu-id="13623-143">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="13623-143">The description of the policy.</span></span>|
|<span data-ttu-id="13623-144">displayName</span><span class="sxs-lookup"><span data-stu-id="13623-144">displayName</span></span>|<span data-ttu-id="13623-145">Строка</span><span class="sxs-lookup"><span data-stu-id="13623-145">String</span></span>|<span data-ttu-id="13623-146">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="13623-146">The display name of the policy.</span></span>|
|<span data-ttu-id="13623-147">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="13623-147">durationInDays</span></span>|<span data-ttu-id="13623-148">Int32</span><span class="sxs-lookup"><span data-stu-id="13623-148">Int32</span></span>|<span data-ttu-id="13623-149">Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="13623-149">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="13623-150">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13623-150">expirationDateTime</span></span>|<span data-ttu-id="13623-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13623-151">DateTimeOffset</span></span>|<span data-ttu-id="13623-152">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="13623-152">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="13623-153">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="13623-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13623-154">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13623-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="13623-155">id</span><span class="sxs-lookup"><span data-stu-id="13623-155">id</span></span>|<span data-ttu-id="13623-156">String</span><span class="sxs-lookup"><span data-stu-id="13623-156">String</span></span>| <span data-ttu-id="13623-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13623-157">Read-only.</span></span>|
|<span data-ttu-id="13623-158">isEnabled</span><span class="sxs-lookup"><span data-stu-id="13623-158">isEnabled</span></span>|<span data-ttu-id="13623-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="13623-159">Boolean</span></span>|<span data-ttu-id="13623-160">Может ли эта политика использоваться для новых запросов.</span><span class="sxs-lookup"><span data-stu-id="13623-160">Can this policy be used for new requests.</span></span>|
|<span data-ttu-id="13623-161">модифиедби</span><span class="sxs-lookup"><span data-stu-id="13623-161">modifiedBy</span></span>|<span data-ttu-id="13623-162">String</span><span class="sxs-lookup"><span data-stu-id="13623-162">String</span></span>|<span data-ttu-id="13623-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13623-163">Read-only.</span></span>|
|<span data-ttu-id="13623-164">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13623-164">modifiedDateTime</span></span>|<span data-ttu-id="13623-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13623-165">DateTimeOffset</span></span>|<span data-ttu-id="13623-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13623-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="13623-168">Связи</span><span class="sxs-lookup"><span data-stu-id="13623-168">Relationships</span></span>

| <span data-ttu-id="13623-169">Связь</span><span class="sxs-lookup"><span data-stu-id="13623-169">Relationship</span></span> | <span data-ttu-id="13623-170">Тип</span><span class="sxs-lookup"><span data-stu-id="13623-170">Type</span></span>        | <span data-ttu-id="13623-171">Описание</span><span class="sxs-lookup"><span data-stu-id="13623-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13623-172">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="13623-172">accessPackage</span></span>|[<span data-ttu-id="13623-173">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="13623-173">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="13623-174">Пакет Access с этой политикой.</span><span class="sxs-lookup"><span data-stu-id="13623-174">The access package with this policy.</span></span> <span data-ttu-id="13623-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13623-175">Read-only.</span></span> <span data-ttu-id="13623-176">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="13623-176">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13623-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13623-177">JSON representation</span></span>

<span data-ttu-id="13623-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13623-178">The following is a JSON representation of the resource.</span></span>

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
    "isEnabled": false,
    "canExtend": false,
    "durationInDays": 365
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
