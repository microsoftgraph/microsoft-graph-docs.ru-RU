---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM). Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a0429de2cacc816eaf1a603a29a08897650da6e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971923"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="c7ca9-104">Тип ресурса governanceResource</span><span class="sxs-lookup"><span data-stu-id="c7ca9-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ca9-105">Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="c7ca9-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="c7ca9-106">Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="c7ca9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c7ca9-107">Methods</span></span>

| <span data-ttu-id="c7ca9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c7ca9-108">Method</span></span>          | <span data-ttu-id="c7ca9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7ca9-109">Return Type</span></span> |<span data-ttu-id="c7ca9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ca9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7ca9-111">List</span><span class="sxs-lookup"><span data-stu-id="c7ca9-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="c7ca9-112">Коллекция [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="c7ca9-113">Перечисление коллекции ресурсов, к которым у запрашивающего есть доступ.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-113">List a collection of resources the requestor has access to.</span></span>|
|<span data-ttu-id="c7ca9-114">[получение](../api/governanceresource-get.md);</span><span class="sxs-lookup"><span data-stu-id="c7ca9-114">[Get](../api/governanceresource-get.md)</span></span> | [<span data-ttu-id="c7ca9-115">governanceResource</span><span class="sxs-lookup"><span data-stu-id="c7ca9-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="c7ca9-116">Чтение свойств и связей объекта ресурса, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="c7ca9-117">Зарегистрировать</span><span class="sxs-lookup"><span data-stu-id="c7ca9-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="c7ca9-118">Регистрация неуправляемой подписки Azure или группы управления для службы управления информационными данными.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="c7ca9-119">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживаются в `roleDefinitions` наборе сущностей в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="c7ca9-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7ca9-120">Properties</span></span>
| <span data-ttu-id="c7ca9-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ca9-121">Property</span></span>          |<span data-ttu-id="c7ca9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ca9-122">Type</span></span>         |<span data-ttu-id="c7ca9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ca9-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="c7ca9-124">id</span><span class="sxs-lookup"><span data-stu-id="c7ca9-124">id</span></span>                 |<span data-ttu-id="c7ca9-125">String</span><span class="sxs-lookup"><span data-stu-id="c7ca9-125">String</span></span>     |<span data-ttu-id="c7ca9-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-126">The id of the resource.</span></span> <span data-ttu-id="c7ca9-127">Он указан в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-127">It is in GUID format.</span></span>|
|<span data-ttu-id="c7ca9-128">externalId</span><span class="sxs-lookup"><span data-stu-id="c7ca9-128">externalId</span></span>           |<span data-ttu-id="c7ca9-129">String</span><span class="sxs-lookup"><span data-stu-id="c7ca9-129">String</span></span>   |<span data-ttu-id="c7ca9-130">Внешний идентификатор ресурса, представляющий его исходный идентификатор во внешней системе.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="c7ca9-131">Например, внешний идентификатор ресурса подписки может иметь значение "/Subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="c7ca9-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="c7ca9-132">type</span><span class="sxs-lookup"><span data-stu-id="c7ca9-132">type</span></span>               |<span data-ttu-id="c7ca9-133">String</span><span class="sxs-lookup"><span data-stu-id="c7ca9-133">String</span></span>     |<span data-ttu-id="c7ca9-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-134">Required.</span></span> <span data-ttu-id="c7ca9-135">Тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-135">Resource type.</span></span> <span data-ttu-id="c7ca9-136">Например, для ресурсов Azure типом может быть "Subscription", "ResourceGroup", "Microsoft. SQL/Server" и т. д.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="c7ca9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c7ca9-137">displayName</span></span>        |<span data-ttu-id="c7ca9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c7ca9-138">String</span></span>     |<span data-ttu-id="c7ca9-139">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-139">The display name of the resource.</span></span>|
|<span data-ttu-id="c7ca9-140">status</span><span class="sxs-lookup"><span data-stu-id="c7ca9-140">status</span></span>             |<span data-ttu-id="c7ca9-141">String</span><span class="sxs-lookup"><span data-stu-id="c7ca9-141">String</span></span>     |<span data-ttu-id="c7ca9-142">Состояние данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-142">The status of a given resource.</span></span> <span data-ttu-id="c7ca9-143">Например, он может представлять, заблокирован ли ресурс (значения: `Active` / `Locked`).</span><span class="sxs-lookup"><span data-stu-id="c7ca9-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="c7ca9-144">Примечание: это свойство может быть расширено в будущем для поддержки дополнительных сценариев.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="c7ca9-145">Регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="c7ca9-145">registeredDateTime</span></span>|<span data-ttu-id="c7ca9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7ca9-146">DateTimeOffset</span></span>      |<span data-ttu-id="c7ca9-147">Представляет дату и время, когда ресурс регистрируется в PIM.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="c7ca9-148">Регистередрут</span><span class="sxs-lookup"><span data-stu-id="c7ca9-148">registeredRoot</span></span>|<span data-ttu-id="c7ca9-149">String</span><span class="sxs-lookup"><span data-stu-id="c7ca9-149">String</span></span>      |<span data-ttu-id="c7ca9-150">Екстерналид из корневой области ресурса, зарегистрированной в PIM.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="c7ca9-151">В качестве корневой области можно указать родительские, бабушке или более поздние ресурсы предков.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="c7ca9-152">Ролеассигнменткаунт</span><span class="sxs-lookup"><span data-stu-id="c7ca9-152">roleAssignmentCount</span></span>|<span data-ttu-id="c7ca9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ca9-153">Int32</span></span>      |<span data-ttu-id="c7ca9-154">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-154">Optional.</span></span> <span data-ttu-id="c7ca9-155">Число назначений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="c7ca9-156">Чтобы получить свойство, используйте `$select=roleAssignmentCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="c7ca9-157">Роледефинитионкаунт</span><span class="sxs-lookup"><span data-stu-id="c7ca9-157">roleDefinitionCount</span></span>|<span data-ttu-id="c7ca9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ca9-158">Int32</span></span>      |<span data-ttu-id="c7ca9-159">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-159">Optional.</span></span> <span data-ttu-id="c7ca9-160">Количество определений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="c7ca9-161">Чтобы получить свойство, используйте `$select=roleDefinitionCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="c7ca9-162">permissions</span><span class="sxs-lookup"><span data-stu-id="c7ca9-162">permissions</span></span>|[<span data-ttu-id="c7ca9-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="c7ca9-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="c7ca9-164">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-164">Optional.</span></span> <span data-ttu-id="c7ca9-165">Он представляет состояние доступа запрашивающего к ресурсу. Чтобы получить свойство, используйте `$select=permissions` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7ca9-166">Отношения</span><span class="sxs-lookup"><span data-stu-id="c7ca9-166">Relationships</span></span>
| <span data-ttu-id="c7ca9-167">Отношение</span><span class="sxs-lookup"><span data-stu-id="c7ca9-167">Relationship</span></span>   | <span data-ttu-id="c7ca9-168">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ca9-168">Type</span></span>                                         |<span data-ttu-id="c7ca9-169">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ca9-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="c7ca9-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c7ca9-170">roleAssignments</span></span> |<span data-ttu-id="c7ca9-171">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="c7ca9-172">Коллекция назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="c7ca9-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c7ca9-173">roleDefinitions</span></span> |<span data-ttu-id="c7ca9-174">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="c7ca9-175">Коллекция ролей дефинтионс для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="c7ca9-176">Ролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="c7ca9-176">roleAssignmentRequests</span></span> |<span data-ttu-id="c7ca9-177">Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="c7ca9-178">Коллекция запросов назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="c7ca9-179">Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="c7ca9-179">roleSettings</span></span> |<span data-ttu-id="c7ca9-180">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="c7ca9-181">Коллекция параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="c7ca9-182">верхнего</span><span class="sxs-lookup"><span data-stu-id="c7ca9-182">parent</span></span>          |[<span data-ttu-id="c7ca9-183">governanceResource</span><span class="sxs-lookup"><span data-stu-id="c7ca9-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="c7ca9-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-184">Read-only.</span></span> <span data-ttu-id="c7ca9-185">Родительский ресурс.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-185">The parent resource.</span></span> <span data-ttu-id="c7ca9-186">для `pimforazurerbac` сценария может представлять подписку, к которой относится ресурс.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7ca9-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7ca9-187">JSON representation</span></span>

<span data-ttu-id="c7ca9-188">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-188">The following is a JSON representation of the resource.</span></span>

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
