---
title: тип ресурса governanceRoleAssignment
description: Представляет назначение пользователя или группы роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6d9e1b56a503ffdf1bde6bde6a583b78f8a34851
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722309"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="5c790-103">тип ресурса governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c790-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="5c790-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="5c790-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="5c790-105">Представляет назначение пользователя или группы роли.</span><span class="sxs-lookup"><span data-stu-id="5c790-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="5c790-106">Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:</span><span class="sxs-lookup"><span data-stu-id="5c790-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="5c790-107">Активное назначение — представляет прямой или активированный доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5c790-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="5c790-108">Право назначения — представляет промежуточный этап привилегированного доступа к ресурсам между отсутствием доступа и прямым доступом.</span><span class="sxs-lookup"><span data-stu-id="5c790-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="5c790-109">Администраторы могут назначать пользователям или группам заранее, и всякий раз, когда необходим доступ, необходимо получить мгновенный доступ к ресурсу `eligible assignment` `activation` в течение нескольких `eligible assignment` часов.</span><span class="sxs-lookup"><span data-stu-id="5c790-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="5c790-110">После активации будет создано для пользователей или членов группы, чтобы указать `active assignment` активированный статус.</span><span class="sxs-lookup"><span data-stu-id="5c790-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="5c790-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5c790-111">Methods</span></span>

| <span data-ttu-id="5c790-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5c790-112">Method</span></span>          | <span data-ttu-id="5c790-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c790-113">Return Type</span></span> |<span data-ttu-id="5c790-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5c790-114">Description</span></span>|
|:------------|:--------|:--------|
|<span data-ttu-id="5c790-115">[получение](../api/governanceroleassignment-get.md);</span><span class="sxs-lookup"><span data-stu-id="5c790-115">[Get](../api/governanceroleassignment-get.md)</span></span> |  [<span data-ttu-id="5c790-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c790-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="5c790-117">Чтение свойств и связей объекта назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="5c790-118">List</span><span class="sxs-lookup"><span data-stu-id="5c790-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="5c790-119">[коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5c790-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="5c790-120">Список набор назначений ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5c790-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="5c790-121">Экспорт</span><span class="sxs-lookup"><span data-stu-id="5c790-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="5c790-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="5c790-122">octet-stream</span></span> |<span data-ttu-id="5c790-123">Скачайте коллекцию назначений ролей на ресурсе и сохраните в качестве `.csv` файла.</span><span class="sxs-lookup"><span data-stu-id="5c790-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="5c790-124">Нет `POST` , или операции `PUT` `PATCH` `DELETE` поддерживаются в `roleAssignments` наборе сущности.</span><span class="sxs-lookup"><span data-stu-id="5c790-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="5c790-125">Любые операции по созданию, обновлению и удаляемой работе `governanceRoleAssignment` делаются `governanceRoleAssignmentRequest` путем .</span><span class="sxs-lookup"><span data-stu-id="5c790-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="5c790-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c790-126">Properties</span></span>
| <span data-ttu-id="5c790-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c790-127">Property</span></span>  | <span data-ttu-id="5c790-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5c790-128">Type</span></span>      |<span data-ttu-id="5c790-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5c790-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="5c790-130">id</span><span class="sxs-lookup"><span data-stu-id="5c790-130">id</span></span>         |<span data-ttu-id="5c790-131">String</span><span class="sxs-lookup"><span data-stu-id="5c790-131">String</span></span>     |<span data-ttu-id="5c790-132">ID назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5c790-132">The ID of the role assignment.</span></span> <span data-ttu-id="5c790-133">Он находится в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="5c790-133">It is in GUID format.</span></span>|
|<span data-ttu-id="5c790-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="5c790-134">resourceId</span></span> |<span data-ttu-id="5c790-135">String</span><span class="sxs-lookup"><span data-stu-id="5c790-135">String</span></span>     |<span data-ttu-id="5c790-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c790-136">Required.</span></span> <span data-ttu-id="5c790-137">ID ресурса, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="5c790-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5c790-138">roleDefinitionId</span></span>|<span data-ttu-id="5c790-139">String</span><span class="sxs-lookup"><span data-stu-id="5c790-139">String</span></span>|<span data-ttu-id="5c790-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c790-140">Required.</span></span> <span data-ttu-id="5c790-141">ID определения роли, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="5c790-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="5c790-142">subjectId</span></span>|<span data-ttu-id="5c790-143">String</span><span class="sxs-lookup"><span data-stu-id="5c790-143">String</span></span>       |<span data-ttu-id="5c790-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c790-144">Required.</span></span> <span data-ttu-id="5c790-145">ID субъекта, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="5c790-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="5c790-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="5c790-147">String</span><span class="sxs-lookup"><span data-stu-id="5c790-147">String</span></span>|<span data-ttu-id="5c790-148">Если это и создано из-за активации `active assignment` на , он представляет собой `eligible assignment` ID `eligible assignment` этого; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="5c790-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="5c790-149">externalId</span><span class="sxs-lookup"><span data-stu-id="5c790-149">externalId</span></span>   |<span data-ttu-id="5c790-150">String</span><span class="sxs-lookup"><span data-stu-id="5c790-150">String</span></span>     |<span data-ttu-id="5c790-151">Внешний ID ресурса, который используется для определения назначения роли в поставщике.</span><span class="sxs-lookup"><span data-stu-id="5c790-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="5c790-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5c790-152">startDateTime</span></span>|<span data-ttu-id="5c790-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c790-153">DateTimeOffset</span></span>|<span data-ttu-id="5c790-154">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5c790-154">The start time of the role assignment.</span></span> <span data-ttu-id="5c790-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5c790-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c790-156">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5c790-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5c790-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5c790-157">endDateTime</span></span>|<span data-ttu-id="5c790-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c790-158">DateTimeOffset</span></span>|<span data-ttu-id="5c790-159">Для назначения непостоянных ролей это время, когда срок действия назначения роли истекает.</span><span class="sxs-lookup"><span data-stu-id="5c790-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="5c790-160">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5c790-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c790-161">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5c790-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5c790-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5c790-162">assignmentState</span></span>|<span data-ttu-id="5c790-163">String</span><span class="sxs-lookup"><span data-stu-id="5c790-163">String</span></span>  |<span data-ttu-id="5c790-164">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="5c790-164">The state of the assignment.</span></span> <span data-ttu-id="5c790-165">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="5c790-165">The value can be</span></span> <ul><li> <span data-ttu-id="5c790-166">`Eligible` для назначения</span><span class="sxs-lookup"><span data-stu-id="5c790-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="5c790-167">`Active` - если оно непосредственно назначено администраторами или активировано при назначении, назначенное `Active` пользователями.</span><span class="sxs-lookup"><span data-stu-id="5c790-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="5c790-168">memberType</span><span class="sxs-lookup"><span data-stu-id="5c790-168">memberType</span></span>|<span data-ttu-id="5c790-169">String</span><span class="sxs-lookup"><span data-stu-id="5c790-169">String</span></span>      |<span data-ttu-id="5c790-170">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="5c790-170">The type of member.</span></span> <span data-ttu-id="5c790-171">Значение может быть:</span><span class="sxs-lookup"><span data-stu-id="5c790-171">The value can be:</span></span> <ul><li><span data-ttu-id="5c790-172">`Inherited` — назначение роли наследуется из области родительского ресурса</span><span class="sxs-lookup"><span data-stu-id="5c790-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="5c790-173">`Group`— назначение роли не наследуется, а происходит от членства в групповом назначении</span><span class="sxs-lookup"><span data-stu-id="5c790-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="5c790-174">`User` — назначение роли не наследуется или не наследуется групповым назначением.</span><span class="sxs-lookup"><span data-stu-id="5c790-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="5c790-175">Связи</span><span class="sxs-lookup"><span data-stu-id="5c790-175">Relationships</span></span>
| <span data-ttu-id="5c790-176">Связь</span><span class="sxs-lookup"><span data-stu-id="5c790-176">Relationship</span></span> | <span data-ttu-id="5c790-177">Тип</span><span class="sxs-lookup"><span data-stu-id="5c790-177">Type</span></span>   |<span data-ttu-id="5c790-178">Описание</span><span class="sxs-lookup"><span data-stu-id="5c790-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c790-179">resource</span><span class="sxs-lookup"><span data-stu-id="5c790-179">resource</span></span>|[<span data-ttu-id="5c790-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="5c790-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="5c790-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c790-181">Read-only.</span></span> <span data-ttu-id="5c790-182">Ресурс, связанный с назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="5c790-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5c790-183">roleDefinition</span></span>|[<span data-ttu-id="5c790-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5c790-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="5c790-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c790-185">Read-only.</span></span> <span data-ttu-id="5c790-186">Определение роли, связанное с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="5c790-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="5c790-187">subject</span><span class="sxs-lookup"><span data-stu-id="5c790-187">subject</span></span>|[<span data-ttu-id="5c790-188">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="5c790-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="5c790-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c790-189">Read-only.</span></span> <span data-ttu-id="5c790-190">Тема, связанная с назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="5c790-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="5c790-191">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c790-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="5c790-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c790-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="5c790-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c790-193">Read-only.</span></span> <span data-ttu-id="5c790-194">Если это и `active assignment` создается из-за активации на объекте, он представляет `eligible assignment` объект `eligible assignment` этого; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="5c790-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c790-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c790-195">JSON representation</span></span>

<span data-ttu-id="5c790-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c790-196">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


