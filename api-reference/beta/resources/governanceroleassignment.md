---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9c5ea36bab1edd453e0fceb51324891b45b70167
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497596"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="a8dc2-103">Тип ресурса governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a8dc2-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="a8dc2-104">Пространство имен: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a8dc2-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="a8dc2-105">Представляет назначение роли пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="a8dc2-106">Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:</span><span class="sxs-lookup"><span data-stu-id="a8dc2-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="a8dc2-107">Активное назначение — представляет прямой/активированный доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="a8dc2-108">Подходящие назначения — представляет промежуточный этап привилегированного доступа к ресурсам, между отсутствием доступа и прямым доступом.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="a8dc2-109">Администраторы могут заранее назначать пользователей и группы `eligible assignment` , а при необходимости `activation` `eligible assignment` получить доступ к ресурсу в течение нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="a8dc2-110">После активации `active assignment` будет создана группа для пользователей и членов группы, указывающая состояние активации.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="a8dc2-111">Методы</span><span class="sxs-lookup"><span data-stu-id="a8dc2-111">Methods</span></span>

| <span data-ttu-id="a8dc2-112">Метод</span><span class="sxs-lookup"><span data-stu-id="a8dc2-112">Method</span></span>          | <span data-ttu-id="a8dc2-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8dc2-113">Return Type</span></span> |<span data-ttu-id="a8dc2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a8dc2-114">Description</span></span>|
|:------------|:--------|:--------|
|<span data-ttu-id="a8dc2-115">[получение](../api/governanceroleassignment-get.md);</span><span class="sxs-lookup"><span data-stu-id="a8dc2-115">[Get](../api/governanceroleassignment-get.md)</span></span> |  [<span data-ttu-id="a8dc2-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a8dc2-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="a8dc2-117">Чтение свойств и связей объекта назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="a8dc2-118">List</span><span class="sxs-lookup"><span data-stu-id="a8dc2-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="a8dc2-119">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a8dc2-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="a8dc2-120">Перечисление коллекции назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="a8dc2-121">Экспорт</span><span class="sxs-lookup"><span data-stu-id="a8dc2-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="a8dc2-122">поток в октетах</span><span class="sxs-lookup"><span data-stu-id="a8dc2-122">octet-stream</span></span> |<span data-ttu-id="a8dc2-123">Скачайте коллекцию назначений ролей для ресурса и сохраните ее `.csv` в виде файла.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="a8dc2-124">`PUT` `POST` `roleAssignments` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH`</span><span class="sxs-lookup"><span data-stu-id="a8dc2-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="a8dc2-125">Все операции по `governanceRoleAssignment` созданию, обновлению и удалению выполняются `governanceRoleAssignmentRequest`.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="a8dc2-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8dc2-126">Properties</span></span>
| <span data-ttu-id="a8dc2-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8dc2-127">Property</span></span>  | <span data-ttu-id="a8dc2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a8dc2-128">Type</span></span>      |<span data-ttu-id="a8dc2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a8dc2-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a8dc2-130">id</span><span class="sxs-lookup"><span data-stu-id="a8dc2-130">id</span></span>         |<span data-ttu-id="a8dc2-131">Строка</span><span class="sxs-lookup"><span data-stu-id="a8dc2-131">String</span></span>     |<span data-ttu-id="a8dc2-132">Идентификатор назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-132">The ID of the role assignment.</span></span> <span data-ttu-id="a8dc2-133">Он указан в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-133">It is in GUID format.</span></span>|
|<span data-ttu-id="a8dc2-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="a8dc2-134">resourceId</span></span> |<span data-ttu-id="a8dc2-135">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-135">String</span></span>     |<span data-ttu-id="a8dc2-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-136">Required.</span></span> <span data-ttu-id="a8dc2-137">Идентификатор ресурса, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="a8dc2-138">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="a8dc2-138">roleDefinitionId</span></span>|<span data-ttu-id="a8dc2-139">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-139">String</span></span>|<span data-ttu-id="a8dc2-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-140">Required.</span></span> <span data-ttu-id="a8dc2-141">Идентификатор определения роли, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="a8dc2-142">субжектид</span><span class="sxs-lookup"><span data-stu-id="a8dc2-142">subjectId</span></span>|<span data-ttu-id="a8dc2-143">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-143">String</span></span>       |<span data-ttu-id="a8dc2-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-144">Required.</span></span> <span data-ttu-id="a8dc2-145">ИДЕНТИФИКАТОР субъекта, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="a8dc2-146">линкеделигиблеролеассигнментид</span><span class="sxs-lookup"><span data-stu-id="a8dc2-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="a8dc2-147">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-147">String</span></span>|<span data-ttu-id="a8dc2-148">Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет идентификатор этого `eligible assignment`объекта; В противном случае — `null`значение.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="a8dc2-149">externalId</span><span class="sxs-lookup"><span data-stu-id="a8dc2-149">externalId</span></span>   |<span data-ttu-id="a8dc2-150">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-150">String</span></span>     |<span data-ttu-id="a8dc2-151">Внешний идентификатор — ресурс, который используется для идентификации назначения роли в поставщике.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="a8dc2-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dc2-152">startDateTime</span></span>|<span data-ttu-id="a8dc2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8dc2-153">DateTimeOffset</span></span>|<span data-ttu-id="a8dc2-154">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-154">The start time of the role assignment.</span></span> <span data-ttu-id="a8dc2-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a8dc2-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a8dc2-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a8dc2-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dc2-157">endDateTime</span></span>|<span data-ttu-id="a8dc2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8dc2-158">DateTimeOffset</span></span>|<span data-ttu-id="a8dc2-159">Для назначения непостоянных ролей это время истечения срока действия назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="a8dc2-160">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a8dc2-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a8dc2-161">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a8dc2-162">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="a8dc2-162">assignmentState</span></span>|<span data-ttu-id="a8dc2-163">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-163">String</span></span>  |<span data-ttu-id="a8dc2-164">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-164">The state of the assignment.</span></span> <span data-ttu-id="a8dc2-165">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="a8dc2-165">The value can be</span></span> <ul><li> <span data-ttu-id="a8dc2-166">`Eligible`для подходящего назначения</span><span class="sxs-lookup"><span data-stu-id="a8dc2-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="a8dc2-167">`Active`— Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="a8dc2-168">мембертипе</span><span class="sxs-lookup"><span data-stu-id="a8dc2-168">memberType</span></span>|<span data-ttu-id="a8dc2-169">String</span><span class="sxs-lookup"><span data-stu-id="a8dc2-169">String</span></span>      |<span data-ttu-id="a8dc2-170">Тип члена.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-170">The type of member.</span></span> <span data-ttu-id="a8dc2-171">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="a8dc2-171">The value can be:</span></span> <ul><li><span data-ttu-id="a8dc2-172">`Inherited`— назначение роли наследуется от родительской области ресурса</span><span class="sxs-lookup"><span data-stu-id="a8dc2-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="a8dc2-173">`Group`— назначение роли не наследуется, но поступает из группы назначения групп.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="a8dc2-174">`User`— назначение роли не является ни унаследованным, ни назначением группы.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="a8dc2-175">Связи</span><span class="sxs-lookup"><span data-stu-id="a8dc2-175">Relationships</span></span>
| <span data-ttu-id="a8dc2-176">Связь</span><span class="sxs-lookup"><span data-stu-id="a8dc2-176">Relationship</span></span> | <span data-ttu-id="a8dc2-177">Тип</span><span class="sxs-lookup"><span data-stu-id="a8dc2-177">Type</span></span>   |<span data-ttu-id="a8dc2-178">Описание</span><span class="sxs-lookup"><span data-stu-id="a8dc2-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8dc2-179">resource</span><span class="sxs-lookup"><span data-stu-id="a8dc2-179">resource</span></span>|[<span data-ttu-id="a8dc2-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="a8dc2-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="a8dc2-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-181">Read-only.</span></span> <span data-ttu-id="a8dc2-182">Ресурс, связанный с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="a8dc2-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a8dc2-183">roleDefinition</span></span>|[<span data-ttu-id="a8dc2-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a8dc2-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="a8dc2-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-185">Read-only.</span></span> <span data-ttu-id="a8dc2-186">Определение роли, связанное с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="a8dc2-187">subject</span><span class="sxs-lookup"><span data-stu-id="a8dc2-187">subject</span></span>|[<span data-ttu-id="a8dc2-188">говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="a8dc2-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="a8dc2-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-189">Read-only.</span></span> <span data-ttu-id="a8dc2-190">Тема, связанная с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="a8dc2-191">линкеделигиблеролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a8dc2-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="a8dc2-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a8dc2-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="a8dc2-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-193">Read-only.</span></span> <span data-ttu-id="a8dc2-194">Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет объект этого `eligible assignment`объекта; В противном случае — `null`значение.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8dc2-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8dc2-195">JSON representation</span></span>

<span data-ttu-id="a8dc2-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8dc2-196">Here is a JSON representation of the resource.</span></span>


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
