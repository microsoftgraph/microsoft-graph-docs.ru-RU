---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 518fbe18fcd09b1b4cc9730c6b7f0112adabfeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971895"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="4d735-103">Тип ресурса governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4d735-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d735-104">Представляет назначение роли пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="4d735-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="4d735-105">Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:</span><span class="sxs-lookup"><span data-stu-id="4d735-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="4d735-106">Активное назначение — представляет прямой/активированный доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4d735-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="4d735-107">Подходящие назначения — представляет промежуточный этап привилегированного доступа к ресурсам, между отсутствием доступа и прямым доступом.</span><span class="sxs-lookup"><span data-stu-id="4d735-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="4d735-108">Администраторы могут заранее назначать пользователей и группы `eligible assignment` , а при необходимости `activation` `eligible assignment` получить доступ к ресурсу в течение нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="4d735-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="4d735-109">После активации `active assignment` будет создана группа для пользователей и членов группы, указывающая состояние активации.</span><span class="sxs-lookup"><span data-stu-id="4d735-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="4d735-110">Методы</span><span class="sxs-lookup"><span data-stu-id="4d735-110">Methods</span></span>

| <span data-ttu-id="4d735-111">Метод</span><span class="sxs-lookup"><span data-stu-id="4d735-111">Method</span></span>          | <span data-ttu-id="4d735-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d735-112">Return Type</span></span> |<span data-ttu-id="4d735-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4d735-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="4d735-114">Получение</span><span class="sxs-lookup"><span data-stu-id="4d735-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="4d735-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4d735-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="4d735-116">Чтение свойств и связей объекта назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="4d735-117">List</span><span class="sxs-lookup"><span data-stu-id="4d735-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="4d735-118">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4d735-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="4d735-119">Перечисление коллекции назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d735-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="4d735-120">Экспорт</span><span class="sxs-lookup"><span data-stu-id="4d735-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="4d735-121">поток в октетах</span><span class="sxs-lookup"><span data-stu-id="4d735-121">octet-stream</span></span> |<span data-ttu-id="4d735-122">Скачайте коллекцию назначений ролей для ресурса и сохраните ее `.csv` в виде файла.</span><span class="sxs-lookup"><span data-stu-id="4d735-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="4d735-123">`PUT` `POST` `roleAssignments` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH`</span><span class="sxs-lookup"><span data-stu-id="4d735-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="4d735-124">Все операции по `governanceRoleAssignment` созданию, обновлению и удалению выполняются `governanceRoleAssignmentRequest`.</span><span class="sxs-lookup"><span data-stu-id="4d735-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="4d735-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d735-125">Properties</span></span>
| <span data-ttu-id="4d735-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d735-126">Property</span></span>  | <span data-ttu-id="4d735-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4d735-127">Type</span></span>      |<span data-ttu-id="4d735-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4d735-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4d735-129">id</span><span class="sxs-lookup"><span data-stu-id="4d735-129">id</span></span>         |<span data-ttu-id="4d735-130">Строка</span><span class="sxs-lookup"><span data-stu-id="4d735-130">String</span></span>     |<span data-ttu-id="4d735-131">Идентификатор назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-131">The ID of the role assignment.</span></span> <span data-ttu-id="4d735-132">Он указан в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="4d735-132">It is in GUID format.</span></span>|
|<span data-ttu-id="4d735-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d735-133">resourceId</span></span> |<span data-ttu-id="4d735-134">String</span><span class="sxs-lookup"><span data-stu-id="4d735-134">String</span></span>     |<span data-ttu-id="4d735-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d735-135">Required.</span></span> <span data-ttu-id="4d735-136">Идентификатор ресурса, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="4d735-137">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4d735-137">roleDefinitionId</span></span>|<span data-ttu-id="4d735-138">String</span><span class="sxs-lookup"><span data-stu-id="4d735-138">String</span></span>|<span data-ttu-id="4d735-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d735-139">Required.</span></span> <span data-ttu-id="4d735-140">Идентификатор определения роли, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="4d735-141">Субжектид</span><span class="sxs-lookup"><span data-stu-id="4d735-141">subjectId</span></span>|<span data-ttu-id="4d735-142">String</span><span class="sxs-lookup"><span data-stu-id="4d735-142">String</span></span>       |<span data-ttu-id="4d735-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d735-143">Required.</span></span> <span data-ttu-id="4d735-144">ИДЕНТИФИКАТОР субъекта, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="4d735-145">Линкеделигиблеролеассигнментид</span><span class="sxs-lookup"><span data-stu-id="4d735-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="4d735-146">String</span><span class="sxs-lookup"><span data-stu-id="4d735-146">String</span></span>|<span data-ttu-id="4d735-147">Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет идентификатор этого `eligible assignment`объекта; В противном случае — `null`значение.</span><span class="sxs-lookup"><span data-stu-id="4d735-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="4d735-148">externalId</span><span class="sxs-lookup"><span data-stu-id="4d735-148">externalId</span></span>   |<span data-ttu-id="4d735-149">String</span><span class="sxs-lookup"><span data-stu-id="4d735-149">String</span></span>     |<span data-ttu-id="4d735-150">Внешний идентификатор — ресурс, который используется для идентификации назначения роли в поставщике.</span><span class="sxs-lookup"><span data-stu-id="4d735-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="4d735-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4d735-151">startDateTime</span></span>|<span data-ttu-id="4d735-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d735-152">DateTimeOffset</span></span>|<span data-ttu-id="4d735-153">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-153">The start time of the role assignment.</span></span> <span data-ttu-id="4d735-154">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4d735-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d735-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4d735-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4d735-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4d735-156">endDateTime</span></span>|<span data-ttu-id="4d735-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d735-157">DateTimeOffset</span></span>|<span data-ttu-id="4d735-158">Для назначения непостоянных ролей это время истечения срока действия назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="4d735-159">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4d735-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d735-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4d735-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4d735-161">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4d735-161">assignmentState</span></span>|<span data-ttu-id="4d735-162">String</span><span class="sxs-lookup"><span data-stu-id="4d735-162">String</span></span>  |<span data-ttu-id="4d735-163">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="4d735-163">The state of the assignment.</span></span> <span data-ttu-id="4d735-164">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="4d735-164">The value can be</span></span> <ul><li> <span data-ttu-id="4d735-165">`Eligible`для подходящего назначения</span><span class="sxs-lookup"><span data-stu-id="4d735-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="4d735-166">`Active`— Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="4d735-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="4d735-167">Мембертипе</span><span class="sxs-lookup"><span data-stu-id="4d735-167">memberType</span></span>|<span data-ttu-id="4d735-168">String</span><span class="sxs-lookup"><span data-stu-id="4d735-168">String</span></span>      |<span data-ttu-id="4d735-169">Тип члена.</span><span class="sxs-lookup"><span data-stu-id="4d735-169">The type of member.</span></span> <span data-ttu-id="4d735-170">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="4d735-170">The value can be:</span></span> <ul><li><span data-ttu-id="4d735-171">`Inherited`— назначение роли наследуется от родительской области ресурса</span><span class="sxs-lookup"><span data-stu-id="4d735-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="4d735-172">`Group`— назначение роли не наследуется, но поступает из группы назначения групп.</span><span class="sxs-lookup"><span data-stu-id="4d735-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="4d735-173">`User`— назначение роли не является ни унаследованным, ни назначением группы.</span><span class="sxs-lookup"><span data-stu-id="4d735-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="4d735-174">Отношения</span><span class="sxs-lookup"><span data-stu-id="4d735-174">Relationships</span></span>
| <span data-ttu-id="4d735-175">Отношение</span><span class="sxs-lookup"><span data-stu-id="4d735-175">Relationship</span></span> | <span data-ttu-id="4d735-176">Тип</span><span class="sxs-lookup"><span data-stu-id="4d735-176">Type</span></span>   |<span data-ttu-id="4d735-177">Описание</span><span class="sxs-lookup"><span data-stu-id="4d735-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d735-178">resource</span><span class="sxs-lookup"><span data-stu-id="4d735-178">resource</span></span>|[<span data-ttu-id="4d735-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="4d735-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="4d735-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d735-180">Read-only.</span></span> <span data-ttu-id="4d735-181">Ресурс, связанный с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="4d735-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4d735-182">roleDefinition</span></span>|[<span data-ttu-id="4d735-183">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="4d735-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="4d735-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d735-184">Read-only.</span></span> <span data-ttu-id="4d735-185">Определение роли, связанное с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="4d735-186">subject</span><span class="sxs-lookup"><span data-stu-id="4d735-186">subject</span></span>|[<span data-ttu-id="4d735-187">Говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="4d735-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="4d735-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d735-188">Read-only.</span></span> <span data-ttu-id="4d735-189">Тема, связанная с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="4d735-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="4d735-190">Линкеделигиблеролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="4d735-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="4d735-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4d735-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="4d735-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d735-192">Read-only.</span></span> <span data-ttu-id="4d735-193">Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет объект этого `eligible assignment`объекта; В противном случае — `null`значение.</span><span class="sxs-lookup"><span data-stu-id="4d735-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d735-194">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d735-194">JSON representation</span></span>

<span data-ttu-id="4d735-195">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d735-195">Here is a JSON representation of the resource.</span></span>


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
