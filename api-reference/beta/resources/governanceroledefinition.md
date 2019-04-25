---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547454"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="2c7dc-104">Тип ресурса Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="2c7dc-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="2c7dc-105">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-105">Represents the role definitions.</span></span> <span data-ttu-id="2c7dc-106">Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2c7dc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2c7dc-107">Methods</span></span>

| <span data-ttu-id="2c7dc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2c7dc-108">Method</span></span>          | <span data-ttu-id="2c7dc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c7dc-109">Return Type</span></span> |<span data-ttu-id="2c7dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7dc-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="2c7dc-111">List</span><span class="sxs-lookup"><span data-stu-id="2c7dc-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="2c7dc-112">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2c7dc-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="2c7dc-113">ПереЧисление коллекции определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="2c7dc-114">Получение</span><span class="sxs-lookup"><span data-stu-id="2c7dc-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="2c7dc-115">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="2c7dc-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="2c7dc-116">Считывание свойств и связей объекта определения роли, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="2c7dc-117">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="2c7dc-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c7dc-118">Properties</span></span>
| <span data-ttu-id="2c7dc-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c7dc-119">Property</span></span>  | <span data-ttu-id="2c7dc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2c7dc-120">Type</span></span>      |<span data-ttu-id="2c7dc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7dc-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="2c7dc-122">id</span><span class="sxs-lookup"><span data-stu-id="2c7dc-122">id</span></span>         |<span data-ttu-id="2c7dc-123">String</span><span class="sxs-lookup"><span data-stu-id="2c7dc-123">String</span></span>     |<span data-ttu-id="2c7dc-124">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-124">The id of the role definition.</span></span> |
|<span data-ttu-id="2c7dc-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="2c7dc-125">resourceId</span></span> |<span data-ttu-id="2c7dc-126">String</span><span class="sxs-lookup"><span data-stu-id="2c7dc-126">String</span></span>     |<span data-ttu-id="2c7dc-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-127">Required.</span></span> <span data-ttu-id="2c7dc-128">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="2c7dc-129">externalId</span><span class="sxs-lookup"><span data-stu-id="2c7dc-129">externalId</span></span>   |<span data-ttu-id="2c7dc-130">String</span><span class="sxs-lookup"><span data-stu-id="2c7dc-130">String</span></span>     |<span data-ttu-id="2c7dc-131">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="2c7dc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2c7dc-132">displayName</span></span>|<span data-ttu-id="2c7dc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2c7dc-133">String</span></span>     |<span data-ttu-id="2c7dc-134">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="2c7dc-135">Субжекткаунт</span><span class="sxs-lookup"><span data-stu-id="2c7dc-135">subjectCount</span></span>|<span data-ttu-id="2c7dc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2c7dc-136">Int32</span></span>     |<span data-ttu-id="2c7dc-137">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-137">Optional.</span></span> <span data-ttu-id="2c7dc-138">Количество субъектов, назначенных для роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="2c7dc-139">Он представляет состояние доступа запрашивающего к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="2c7dc-140">Чтобы получить свойство, используйте `$select=subjectCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="2c7dc-141">Елигиблеассигнменткаунт</span><span class="sxs-lookup"><span data-stu-id="2c7dc-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="2c7dc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2c7dc-142">Int32</span></span>|<span data-ttu-id="2c7dc-143">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-143">Optional.</span></span> <span data-ttu-id="2c7dc-144">Число подходящих назначений ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="2c7dc-145">Чтобы получить свойство, используйте `$select=eligibleAssignmentCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="2c7dc-146">Активеассигнменткаунт</span><span class="sxs-lookup"><span data-stu-id="2c7dc-146">activeAssignmentCount</span></span>|<span data-ttu-id="2c7dc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2c7dc-147">Int32</span></span>    |<span data-ttu-id="2c7dc-148">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-148">Optional.</span></span> <span data-ttu-id="2c7dc-149">Количество активных назначений ролей, связанных с определением роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="2c7dc-150">Чтобы получить свойство, используйте `$select=activeAssignmentCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2c7dc-151">Связи</span><span class="sxs-lookup"><span data-stu-id="2c7dc-151">Relationships</span></span>
| <span data-ttu-id="2c7dc-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="2c7dc-152">Relationship</span></span> | <span data-ttu-id="2c7dc-153">Тип</span><span class="sxs-lookup"><span data-stu-id="2c7dc-153">Type</span></span>   |<span data-ttu-id="2c7dc-154">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7dc-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c7dc-155">resource</span><span class="sxs-lookup"><span data-stu-id="2c7dc-155">resource</span></span>|[<span data-ttu-id="2c7dc-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="2c7dc-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="2c7dc-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-157">Read-only.</span></span> <span data-ttu-id="2c7dc-158">Связанный ресурс для определения роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="2c7dc-159">Ролесеттинг</span><span class="sxs-lookup"><span data-stu-id="2c7dc-159">roleSetting</span></span>|[<span data-ttu-id="2c7dc-160">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="2c7dc-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="2c7dc-161">Связанный параметр роли для определения роли.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c7dc-162">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2c7dc-162">JSON representation</span></span>

<span data-ttu-id="2c7dc-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c7dc-163">Here is a JSON representation of the resource.</span></span>

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
