---
title: тип ресурсов governanceResource
description: Представляет ресурсы, которыми может управлять привилегированное управление удостоверениями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e0cf42593a35103996217d1ce18bd9938b48a185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443119"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="786eb-104">тип ресурсов governanceResource</span><span class="sxs-lookup"><span data-stu-id="786eb-104">governanceResource resource type</span></span>

<span data-ttu-id="786eb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786eb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786eb-106">Представляет ресурсы, которыми может управлять привилегированное управление удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="786eb-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="786eb-107">Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.</span><span class="sxs-lookup"><span data-stu-id="786eb-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="786eb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="786eb-108">Methods</span></span>

| <span data-ttu-id="786eb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="786eb-109">Method</span></span>          | <span data-ttu-id="786eb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="786eb-110">Return Type</span></span> |<span data-ttu-id="786eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="786eb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="786eb-112">Список</span><span class="sxs-lookup"><span data-stu-id="786eb-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="786eb-113">[коллекция governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="786eb-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="786eb-114">Перечислить коллекцию ресурсов, к которые имеет доступ запросчик.</span><span class="sxs-lookup"><span data-stu-id="786eb-114">List a collection of resources the requestor has access to.</span></span>|
|<span data-ttu-id="786eb-115">[получение](../api/governanceresource-get.md);</span><span class="sxs-lookup"><span data-stu-id="786eb-115">[Get](../api/governanceresource-get.md)</span></span> | [<span data-ttu-id="786eb-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="786eb-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="786eb-117">Чтение свойств и связей объекта ресурсов, указанного в id.</span><span class="sxs-lookup"><span data-stu-id="786eb-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="786eb-118">Зарегистрировать</span><span class="sxs-lookup"><span data-stu-id="786eb-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="786eb-119">Зарегистрируйте неуправленную подписку или группу управления Azure в службу PIM.</span><span class="sxs-lookup"><span data-stu-id="786eb-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="786eb-120">`POST`Нет, `PUT` `PATCH` `DELETE` поддерживаются в `roleDefinitions` наборе сущности на данный момент.</span><span class="sxs-lookup"><span data-stu-id="786eb-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="786eb-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="786eb-121">Properties</span></span>
| <span data-ttu-id="786eb-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="786eb-122">Property</span></span>          |<span data-ttu-id="786eb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="786eb-123">Type</span></span>         |<span data-ttu-id="786eb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="786eb-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="786eb-125">id</span><span class="sxs-lookup"><span data-stu-id="786eb-125">id</span></span>                 |<span data-ttu-id="786eb-126">String</span><span class="sxs-lookup"><span data-stu-id="786eb-126">String</span></span>     |<span data-ttu-id="786eb-127">Id ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-127">The id of the resource.</span></span> <span data-ttu-id="786eb-128">Он находится в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="786eb-128">It is in GUID format.</span></span>|
|<span data-ttu-id="786eb-129">externalId</span><span class="sxs-lookup"><span data-stu-id="786eb-129">externalId</span></span>           |<span data-ttu-id="786eb-130">String</span><span class="sxs-lookup"><span data-stu-id="786eb-130">String</span></span>   |<span data-ttu-id="786eb-131">Внешний id ресурса, представляющий его исходный id во внешней системе.</span><span class="sxs-lookup"><span data-stu-id="786eb-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="786eb-132">Например, внешний id ресурса подписки может быть "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="786eb-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="786eb-133">type</span><span class="sxs-lookup"><span data-stu-id="786eb-133">type</span></span>               |<span data-ttu-id="786eb-134">String</span><span class="sxs-lookup"><span data-stu-id="786eb-134">String</span></span>     |<span data-ttu-id="786eb-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="786eb-135">Required.</span></span> <span data-ttu-id="786eb-136">Тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-136">Resource type.</span></span> <span data-ttu-id="786eb-137">Например, для ресурсов Azure тип может быть "Подписка", "ResourceGroup", "Microsoft.Sql/server" и т.д.</span><span class="sxs-lookup"><span data-stu-id="786eb-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="786eb-138">displayName</span><span class="sxs-lookup"><span data-stu-id="786eb-138">displayName</span></span>        |<span data-ttu-id="786eb-139">String</span><span class="sxs-lookup"><span data-stu-id="786eb-139">String</span></span>     |<span data-ttu-id="786eb-140">Имя отображения ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-140">The display name of the resource.</span></span>|
|<span data-ttu-id="786eb-141">status</span><span class="sxs-lookup"><span data-stu-id="786eb-141">status</span></span>             |<span data-ttu-id="786eb-142">String</span><span class="sxs-lookup"><span data-stu-id="786eb-142">String</span></span>     |<span data-ttu-id="786eb-143">Состояние данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-143">The status of a given resource.</span></span> <span data-ttu-id="786eb-144">Например, он может представлять, заблокирован ресурс или нет (значения: `Active` / `Locked` ).</span><span class="sxs-lookup"><span data-stu-id="786eb-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="786eb-145">Примечание. Это свойство может быть расширено в будущем, чтобы поддерживать дополнительные сценарии.</span><span class="sxs-lookup"><span data-stu-id="786eb-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="786eb-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="786eb-146">registeredDateTime</span></span>|<span data-ttu-id="786eb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="786eb-147">DateTimeOffset</span></span>      |<span data-ttu-id="786eb-148">Представляет время даты регистрации ресурса в PIM.</span><span class="sxs-lookup"><span data-stu-id="786eb-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="786eb-149">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="786eb-149">registeredRoot</span></span>|<span data-ttu-id="786eb-150">String</span><span class="sxs-lookup"><span data-stu-id="786eb-150">String</span></span>      |<span data-ttu-id="786eb-151">ExternalId корневой области ресурса, зарегистрированной в PIM.</span><span class="sxs-lookup"><span data-stu-id="786eb-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="786eb-152">Корневой областью могут быть родительские, бабушки и дедушки или более высокие ресурсы предка.</span><span class="sxs-lookup"><span data-stu-id="786eb-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="786eb-153">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="786eb-153">roleAssignmentCount</span></span>|<span data-ttu-id="786eb-154">Int32</span><span class="sxs-lookup"><span data-stu-id="786eb-154">Int32</span></span>      |<span data-ttu-id="786eb-155">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="786eb-155">Optional.</span></span> <span data-ttu-id="786eb-156">Количество назначений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="786eb-157">Чтобы получить свойство, используйте его в `$select=roleAssignmentCount` запросе.</span><span class="sxs-lookup"><span data-stu-id="786eb-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="786eb-158">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="786eb-158">roleDefinitionCount</span></span>|<span data-ttu-id="786eb-159">Int32</span><span class="sxs-lookup"><span data-stu-id="786eb-159">Int32</span></span>      |<span data-ttu-id="786eb-160">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="786eb-160">Optional.</span></span> <span data-ttu-id="786eb-161">Количество определений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="786eb-162">Чтобы получить свойство, используйте его в `$select=roleDefinitionCount` запросе.</span><span class="sxs-lookup"><span data-stu-id="786eb-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="786eb-163">permissions</span><span class="sxs-lookup"><span data-stu-id="786eb-163">permissions</span></span>|[<span data-ttu-id="786eb-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="786eb-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="786eb-165">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="786eb-165">Optional.</span></span> <span data-ttu-id="786eb-166">Он представляет состояние доступа запросителя к ресурсу. Чтобы получить свойство, используйте его в `$select=permissions` запросе.</span><span class="sxs-lookup"><span data-stu-id="786eb-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="786eb-167">Связи</span><span class="sxs-lookup"><span data-stu-id="786eb-167">Relationships</span></span>
| <span data-ttu-id="786eb-168">Связь</span><span class="sxs-lookup"><span data-stu-id="786eb-168">Relationship</span></span>   | <span data-ttu-id="786eb-169">Тип</span><span class="sxs-lookup"><span data-stu-id="786eb-169">Type</span></span>                                         |<span data-ttu-id="786eb-170">Описание</span><span class="sxs-lookup"><span data-stu-id="786eb-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="786eb-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="786eb-171">roleAssignments</span></span> |<span data-ttu-id="786eb-172">[коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="786eb-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="786eb-173">Коллекция назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="786eb-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="786eb-174">roleDefinitions</span></span> |<span data-ttu-id="786eb-175">[коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="786eb-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="786eb-176">Коллекция defintions роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="786eb-177">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="786eb-177">roleAssignmentRequests</span></span> |<span data-ttu-id="786eb-178">[коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="786eb-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="786eb-179">Коллекция запросов на назначение ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="786eb-180">roleSettings</span><span class="sxs-lookup"><span data-stu-id="786eb-180">roleSettings</span></span> |<span data-ttu-id="786eb-181">[коллекция governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="786eb-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="786eb-182">Коллекция параметров ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="786eb-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="786eb-183">родитель</span><span class="sxs-lookup"><span data-stu-id="786eb-183">parent</span></span>          |[<span data-ttu-id="786eb-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="786eb-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="786eb-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="786eb-185">Read-only.</span></span> <span data-ttu-id="786eb-186">Родительский ресурс.</span><span class="sxs-lookup"><span data-stu-id="786eb-186">The parent resource.</span></span> <span data-ttu-id="786eb-187">для `pimforazurerbac` сценария он может представлять подписку, к которой принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="786eb-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="786eb-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="786eb-188">JSON representation</span></span>

<span data-ttu-id="786eb-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="786eb-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


