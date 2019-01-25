---
title: Тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528643"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="58f57-104">Тип ресурса governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="58f57-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="58f57-105">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="58f57-105">Represents the role definitions.</span></span> <span data-ttu-id="58f57-106">Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.</span><span class="sxs-lookup"><span data-stu-id="58f57-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="58f57-107">Методы</span><span class="sxs-lookup"><span data-stu-id="58f57-107">Methods</span></span>

| <span data-ttu-id="58f57-108">Метод</span><span class="sxs-lookup"><span data-stu-id="58f57-108">Method</span></span>          | <span data-ttu-id="58f57-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58f57-109">Return Type</span></span> |<span data-ttu-id="58f57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58f57-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="58f57-111">List</span><span class="sxs-lookup"><span data-stu-id="58f57-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="58f57-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="58f57-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="58f57-113">Список коллекцию определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="58f57-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="58f57-114">Get</span><span class="sxs-lookup"><span data-stu-id="58f57-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="58f57-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="58f57-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="58f57-116">Чтение свойства и связи с указанным идентификатором сущности определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="58f57-117">Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживается на `roleDefinitions` набора сущностей в данный момент.</span><span class="sxs-lookup"><span data-stu-id="58f57-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="58f57-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="58f57-118">Properties</span></span>
| <span data-ttu-id="58f57-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="58f57-119">Property</span></span>  | <span data-ttu-id="58f57-120">Тип</span><span class="sxs-lookup"><span data-stu-id="58f57-120">Type</span></span>      |<span data-ttu-id="58f57-121">Описание</span><span class="sxs-lookup"><span data-stu-id="58f57-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="58f57-122">id</span><span class="sxs-lookup"><span data-stu-id="58f57-122">id</span></span>         |<span data-ttu-id="58f57-123">Строка</span><span class="sxs-lookup"><span data-stu-id="58f57-123">String</span></span>     |<span data-ttu-id="58f57-124">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-124">The id of the role definition.</span></span> |
|<span data-ttu-id="58f57-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="58f57-125">resourceId</span></span> |<span data-ttu-id="58f57-126">Строка</span><span class="sxs-lookup"><span data-stu-id="58f57-126">String</span></span>     |<span data-ttu-id="58f57-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58f57-127">Required.</span></span> <span data-ttu-id="58f57-128">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="58f57-129">externalId</span><span class="sxs-lookup"><span data-stu-id="58f57-129">externalId</span></span>   |<span data-ttu-id="58f57-130">String</span><span class="sxs-lookup"><span data-stu-id="58f57-130">String</span></span>     |<span data-ttu-id="58f57-131">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="58f57-132">displayName</span><span class="sxs-lookup"><span data-stu-id="58f57-132">displayName</span></span>|<span data-ttu-id="58f57-133">String</span><span class="sxs-lookup"><span data-stu-id="58f57-133">String</span></span>     |<span data-ttu-id="58f57-134">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="58f57-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="58f57-135">subjectCount</span></span>|<span data-ttu-id="58f57-136">Int32</span><span class="sxs-lookup"><span data-stu-id="58f57-136">Int32</span></span>     |<span data-ttu-id="58f57-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="58f57-137">Optional.</span></span> <span data-ttu-id="58f57-138">Число субъектов, которые были им назначены роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="58f57-139">Он представляет состояние запрашивающего доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="58f57-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="58f57-140">Чтобы получить свойство, рекомендуется использовать явным образом `$select=subjectCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="58f57-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="58f57-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="58f57-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="58f57-142">Int32</span><span class="sxs-lookup"><span data-stu-id="58f57-142">Int32</span></span>|<span data-ttu-id="58f57-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="58f57-143">Optional.</span></span> <span data-ttu-id="58f57-144">Число назначений подходящими ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="58f57-145">Чтобы получить свойство, рекомендуется использовать явным образом `$select=eligibleAssignmentCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="58f57-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="58f57-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="58f57-146">activeAssignmentCount</span></span>|<span data-ttu-id="58f57-147">Int32</span><span class="sxs-lookup"><span data-stu-id="58f57-147">Int32</span></span>    |<span data-ttu-id="58f57-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="58f57-148">Optional.</span></span> <span data-ttu-id="58f57-149">Число назначений active ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="58f57-150">Чтобы получить свойство, рекомендуется использовать явным образом `$select=activeAssignmentCount` в запросе.</span><span class="sxs-lookup"><span data-stu-id="58f57-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="58f57-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="58f57-151">Relationships</span></span>
| <span data-ttu-id="58f57-152">Связь</span><span class="sxs-lookup"><span data-stu-id="58f57-152">Relationship</span></span> | <span data-ttu-id="58f57-153">Тип</span><span class="sxs-lookup"><span data-stu-id="58f57-153">Type</span></span>   |<span data-ttu-id="58f57-154">Описание</span><span class="sxs-lookup"><span data-stu-id="58f57-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58f57-155">resource</span><span class="sxs-lookup"><span data-stu-id="58f57-155">resource</span></span>|[<span data-ttu-id="58f57-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="58f57-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="58f57-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58f57-157">Read-only.</span></span> <span data-ttu-id="58f57-158">Связанные ресурсов для определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="58f57-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="58f57-159">roleSetting</span></span>|[<span data-ttu-id="58f57-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="58f57-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="58f57-161">Параметр связанных ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="58f57-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58f57-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58f57-162">JSON representation</span></span>

<span data-ttu-id="58f57-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58f57-163">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
