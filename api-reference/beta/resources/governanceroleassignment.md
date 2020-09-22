---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: fec241d2152fd4b2cea68159f3eb1c6154bacabe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081694"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="31c35-103">Тип ресурса governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="31c35-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="31c35-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="31c35-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="31c35-105">Представляет назначение роли пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="31c35-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="31c35-106">Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:</span><span class="sxs-lookup"><span data-stu-id="31c35-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="31c35-107">Активное назначение — представляет прямой/активированный доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="31c35-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="31c35-108">Подходящие назначения — представляет промежуточный этап привилегированного доступа к ресурсам, между отсутствием доступа и прямым доступом.</span><span class="sxs-lookup"><span data-stu-id="31c35-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="31c35-109">Администраторы могут заранее назначать пользователей и группы `eligible assignment` , а при необходимости получить доступ к `activation` `eligible assignment` ресурсу в течение нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="31c35-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="31c35-110">После активации `active assignment` будет создана группа для пользователей и членов группы, указывающая состояние активации.</span><span class="sxs-lookup"><span data-stu-id="31c35-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="31c35-111">Методы</span><span class="sxs-lookup"><span data-stu-id="31c35-111">Methods</span></span>

| <span data-ttu-id="31c35-112">Метод</span><span class="sxs-lookup"><span data-stu-id="31c35-112">Method</span></span>          | <span data-ttu-id="31c35-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31c35-113">Return Type</span></span> |<span data-ttu-id="31c35-114">Описание</span><span class="sxs-lookup"><span data-stu-id="31c35-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="31c35-115">Получение</span><span class="sxs-lookup"><span data-stu-id="31c35-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="31c35-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="31c35-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="31c35-117">Чтение свойств и связей объекта назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="31c35-118">Перечисление</span><span class="sxs-lookup"><span data-stu-id="31c35-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="31c35-119">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="31c35-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="31c35-120">Перечисление коллекции назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="31c35-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="31c35-121">Экспорт</span><span class="sxs-lookup"><span data-stu-id="31c35-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="31c35-122">поток в октетах</span><span class="sxs-lookup"><span data-stu-id="31c35-122">octet-stream</span></span> |<span data-ttu-id="31c35-123">Скачайте коллекцию назначений ролей для ресурса и сохраните ее в виде `.csv` файла.</span><span class="sxs-lookup"><span data-stu-id="31c35-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="31c35-124">`POST` `PUT` `PATCH` `DELETE` В наборе сущностей поддерживаются не поддерживаемые операции, а также операции `roleAssignments` .</span><span class="sxs-lookup"><span data-stu-id="31c35-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="31c35-125">Все операции по созданию, обновлению и удалению выполняются `governanceRoleAssignment` `governanceRoleAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="31c35-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="31c35-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="31c35-126">Properties</span></span>
| <span data-ttu-id="31c35-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="31c35-127">Property</span></span>  | <span data-ttu-id="31c35-128">Тип</span><span class="sxs-lookup"><span data-stu-id="31c35-128">Type</span></span>      |<span data-ttu-id="31c35-129">Описание</span><span class="sxs-lookup"><span data-stu-id="31c35-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="31c35-130">id</span><span class="sxs-lookup"><span data-stu-id="31c35-130">id</span></span>         |<span data-ttu-id="31c35-131">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-131">String</span></span>     |<span data-ttu-id="31c35-132">Идентификатор назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-132">The ID of the role assignment.</span></span> <span data-ttu-id="31c35-133">Он указан в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="31c35-133">It is in GUID format.</span></span>|
|<span data-ttu-id="31c35-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="31c35-134">resourceId</span></span> |<span data-ttu-id="31c35-135">String</span><span class="sxs-lookup"><span data-stu-id="31c35-135">String</span></span>     |<span data-ttu-id="31c35-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31c35-136">Required.</span></span> <span data-ttu-id="31c35-137">Идентификатор ресурса, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="31c35-138">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31c35-138">roleDefinitionId</span></span>|<span data-ttu-id="31c35-139">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-139">String</span></span>|<span data-ttu-id="31c35-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31c35-140">Required.</span></span> <span data-ttu-id="31c35-141">Идентификатор определения роли, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="31c35-142">субжектид</span><span class="sxs-lookup"><span data-stu-id="31c35-142">subjectId</span></span>|<span data-ttu-id="31c35-143">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-143">String</span></span>       |<span data-ttu-id="31c35-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31c35-144">Required.</span></span> <span data-ttu-id="31c35-145">ИДЕНТИФИКАТОР субъекта, с которым связано назначение роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="31c35-146">линкеделигиблеролеассигнментид</span><span class="sxs-lookup"><span data-stu-id="31c35-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="31c35-147">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-147">String</span></span>|<span data-ttu-id="31c35-148">Если он `active assignment` создан и создан в результате активации `eligible assignment` , он представляет идентификатор этого объекта `eligible assignment` ; В противном случае — значение `null` .</span><span class="sxs-lookup"><span data-stu-id="31c35-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="31c35-149">externalId</span><span class="sxs-lookup"><span data-stu-id="31c35-149">externalId</span></span>   |<span data-ttu-id="31c35-150">String</span><span class="sxs-lookup"><span data-stu-id="31c35-150">String</span></span>     |<span data-ttu-id="31c35-151">Внешний идентификатор — ресурс, который используется для идентификации назначения роли в поставщике.</span><span class="sxs-lookup"><span data-stu-id="31c35-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="31c35-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31c35-152">startDateTime</span></span>|<span data-ttu-id="31c35-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31c35-153">DateTimeOffset</span></span>|<span data-ttu-id="31c35-154">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-154">The start time of the role assignment.</span></span> <span data-ttu-id="31c35-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="31c35-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31c35-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31c35-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="31c35-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="31c35-157">endDateTime</span></span>|<span data-ttu-id="31c35-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31c35-158">DateTimeOffset</span></span>|<span data-ttu-id="31c35-159">Для назначения непостоянных ролей это время истечения срока действия назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="31c35-160">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="31c35-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31c35-161">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31c35-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="31c35-162">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31c35-162">assignmentState</span></span>|<span data-ttu-id="31c35-163">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-163">String</span></span>  |<span data-ttu-id="31c35-164">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="31c35-164">The state of the assignment.</span></span> <span data-ttu-id="31c35-165">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="31c35-165">The value can be</span></span> <ul><li> <span data-ttu-id="31c35-166">`Eligible` для подходящего назначения</span><span class="sxs-lookup"><span data-stu-id="31c35-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="31c35-167">`Active` — Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="31c35-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="31c35-168">мембертипе</span><span class="sxs-lookup"><span data-stu-id="31c35-168">memberType</span></span>|<span data-ttu-id="31c35-169">Строка</span><span class="sxs-lookup"><span data-stu-id="31c35-169">String</span></span>      |<span data-ttu-id="31c35-170">Тип члена.</span><span class="sxs-lookup"><span data-stu-id="31c35-170">The type of member.</span></span> <span data-ttu-id="31c35-171">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="31c35-171">The value can be:</span></span> <ul><li><span data-ttu-id="31c35-172">`Inherited` — назначение роли наследуется от родительской области ресурса</span><span class="sxs-lookup"><span data-stu-id="31c35-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="31c35-173">`Group`— назначение роли не наследуется, но поступает из группы назначения групп.</span><span class="sxs-lookup"><span data-stu-id="31c35-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="31c35-174">`User` — назначение роли не является ни унаследованным, ни назначением группы.</span><span class="sxs-lookup"><span data-stu-id="31c35-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="31c35-175">Связи</span><span class="sxs-lookup"><span data-stu-id="31c35-175">Relationships</span></span>
| <span data-ttu-id="31c35-176">Связь</span><span class="sxs-lookup"><span data-stu-id="31c35-176">Relationship</span></span> | <span data-ttu-id="31c35-177">Тип</span><span class="sxs-lookup"><span data-stu-id="31c35-177">Type</span></span>   |<span data-ttu-id="31c35-178">Описание</span><span class="sxs-lookup"><span data-stu-id="31c35-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31c35-179">resource</span><span class="sxs-lookup"><span data-stu-id="31c35-179">resource</span></span>|[<span data-ttu-id="31c35-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="31c35-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="31c35-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31c35-181">Read-only.</span></span> <span data-ttu-id="31c35-182">Ресурс, связанный с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="31c35-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31c35-183">roleDefinition</span></span>|[<span data-ttu-id="31c35-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31c35-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="31c35-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31c35-185">Read-only.</span></span> <span data-ttu-id="31c35-186">Определение роли, связанное с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="31c35-187">subject</span><span class="sxs-lookup"><span data-stu-id="31c35-187">subject</span></span>|[<span data-ttu-id="31c35-188">говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="31c35-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="31c35-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31c35-189">Read-only.</span></span> <span data-ttu-id="31c35-190">Тема, связанная с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="31c35-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="31c35-191">линкеделигиблеролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="31c35-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="31c35-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="31c35-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="31c35-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31c35-193">Read-only.</span></span> <span data-ttu-id="31c35-194">Если он `active assignment` создан и создан в результате активации `eligible assignment` , он представляет объект этого объекта `eligible assignment` ; В противном случае — значение `null` .</span><span class="sxs-lookup"><span data-stu-id="31c35-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31c35-195">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31c35-195">JSON representation</span></span>

<span data-ttu-id="31c35-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31c35-196">Here is a JSON representation of the resource.</span></span>


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


