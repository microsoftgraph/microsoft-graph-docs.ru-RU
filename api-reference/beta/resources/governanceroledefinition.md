---
title: Тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842453"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="cd72a-104">Тип ресурса governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cd72a-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="cd72a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd72a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd72a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd72a-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="cd72a-107">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="cd72a-107">Represents the role definitions.</span></span> <span data-ttu-id="cd72a-108">Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.</span><span class="sxs-lookup"><span data-stu-id="cd72a-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="cd72a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="cd72a-109">Methods</span></span>

| <span data-ttu-id="cd72a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="cd72a-110">Method</span></span>          | <span data-ttu-id="cd72a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd72a-111">Return Type</span></span> |<span data-ttu-id="cd72a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd72a-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="cd72a-113">List</span><span class="sxs-lookup"><span data-stu-id="cd72a-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="cd72a-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cd72a-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="cd72a-115">Список коллекцию определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd72a-115">List a collection of role definitions on a resource.</span></span>|
|<span data-ttu-id="cd72a-116">[получение](../api/governanceroledefinition-get.md);</span><span class="sxs-lookup"><span data-stu-id="cd72a-116">[Get](../api/governanceroledefinition-get.md)</span></span> | [<span data-ttu-id="cd72a-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cd72a-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="cd72a-118">Чтение свойства и связи с указанным идентификатором сущности определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="cd72a-119">Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживается на `roleDefinitions` набора сущностей в данный момент.</span><span class="sxs-lookup"><span data-stu-id="cd72a-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="cd72a-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd72a-120">Properties</span></span>
| <span data-ttu-id="cd72a-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd72a-121">Property</span></span>  | <span data-ttu-id="cd72a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="cd72a-122">Type</span></span>      |<span data-ttu-id="cd72a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cd72a-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="cd72a-124">id</span><span class="sxs-lookup"><span data-stu-id="cd72a-124">id</span></span>         |<span data-ttu-id="cd72a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="cd72a-125">String</span></span>     |<span data-ttu-id="cd72a-126">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-126">The id of the role definition.</span></span> |
|<span data-ttu-id="cd72a-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="cd72a-127">resourceId</span></span> |<span data-ttu-id="cd72a-128">Строка</span><span class="sxs-lookup"><span data-stu-id="cd72a-128">String</span></span>     |<span data-ttu-id="cd72a-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd72a-129">Required.</span></span> <span data-ttu-id="cd72a-130">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="cd72a-131">externalId</span><span class="sxs-lookup"><span data-stu-id="cd72a-131">externalId</span></span>   |<span data-ttu-id="cd72a-132">String</span><span class="sxs-lookup"><span data-stu-id="cd72a-132">String</span></span>     |<span data-ttu-id="cd72a-133">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="cd72a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cd72a-134">displayName</span></span>|<span data-ttu-id="cd72a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="cd72a-135">String</span></span>     |<span data-ttu-id="cd72a-136">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="cd72a-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="cd72a-137">subjectCount</span></span>|<span data-ttu-id="cd72a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cd72a-138">Int32</span></span>     |<span data-ttu-id="cd72a-139">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="cd72a-139">Optional.</span></span> <span data-ttu-id="cd72a-140">Число субъектов, которые были им назначены роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="cd72a-141">Он представляет состояние запрашивающего доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="cd72a-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="cd72a-142">Чтобы получить свойство, рекомендуется использовать явным образом `$select=subjectCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="cd72a-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="cd72a-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="cd72a-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="cd72a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cd72a-144">Int32</span></span>|<span data-ttu-id="cd72a-145">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="cd72a-145">Optional.</span></span> <span data-ttu-id="cd72a-146">Число назначений подходящими ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="cd72a-147">Чтобы получить свойство, рекомендуется использовать явным образом `$select=eligibleAssignmentCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="cd72a-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="cd72a-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="cd72a-148">activeAssignmentCount</span></span>|<span data-ttu-id="cd72a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="cd72a-149">Int32</span></span>    |<span data-ttu-id="cd72a-150">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="cd72a-150">Optional.</span></span> <span data-ttu-id="cd72a-151">Число назначений active ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="cd72a-152">Чтобы получить свойство, рекомендуется использовать явным образом `$select=activeAssignmentCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="cd72a-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="cd72a-153">Связи</span><span class="sxs-lookup"><span data-stu-id="cd72a-153">Relationships</span></span>
| <span data-ttu-id="cd72a-154">Связь</span><span class="sxs-lookup"><span data-stu-id="cd72a-154">Relationship</span></span> | <span data-ttu-id="cd72a-155">Тип</span><span class="sxs-lookup"><span data-stu-id="cd72a-155">Type</span></span>   |<span data-ttu-id="cd72a-156">Описание</span><span class="sxs-lookup"><span data-stu-id="cd72a-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd72a-157">resource</span><span class="sxs-lookup"><span data-stu-id="cd72a-157">resource</span></span>|[<span data-ttu-id="cd72a-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="cd72a-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="cd72a-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd72a-159">Read-only.</span></span> <span data-ttu-id="cd72a-160">Связанные ресурсов для определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="cd72a-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="cd72a-161">roleSetting</span></span>|[<span data-ttu-id="cd72a-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="cd72a-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="cd72a-163">Параметр связанных ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="cd72a-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd72a-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd72a-164">JSON representation</span></span>

<span data-ttu-id="cd72a-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd72a-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
