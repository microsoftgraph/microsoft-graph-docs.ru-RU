---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM). Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d2ce70da20a3a976acc567ee8138cc0b0dcaffb2
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219251"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="34de9-104">Тип ресурса governanceResource</span><span class="sxs-lookup"><span data-stu-id="34de9-104">governanceResource resource type</span></span>

<span data-ttu-id="34de9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34de9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34de9-106">Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="34de9-106">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="34de9-107">Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.</span><span class="sxs-lookup"><span data-stu-id="34de9-107">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="34de9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="34de9-108">Methods</span></span>

| <span data-ttu-id="34de9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="34de9-109">Method</span></span>          | <span data-ttu-id="34de9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34de9-110">Return Type</span></span> |<span data-ttu-id="34de9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34de9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34de9-112">List</span><span class="sxs-lookup"><span data-stu-id="34de9-112">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="34de9-113">Коллекция [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="34de9-113">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="34de9-114">Перечисление коллекции ресурсов, к которым у запрашивающего есть доступ.</span><span class="sxs-lookup"><span data-stu-id="34de9-114">List a collection of resources the requestor has access to.</span></span>|
|<span data-ttu-id="34de9-115">[получение](../api/governanceresource-get.md);</span><span class="sxs-lookup"><span data-stu-id="34de9-115">[Get](../api/governanceresource-get.md)</span></span> | [<span data-ttu-id="34de9-116">governanceResource</span><span class="sxs-lookup"><span data-stu-id="34de9-116">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="34de9-117">Чтение свойств и связей объекта ресурса, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="34de9-117">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="34de9-118">Зарегистрировать</span><span class="sxs-lookup"><span data-stu-id="34de9-118">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="34de9-119">Регистрация неуправляемой подписки Azure или группы управления для службы управления информационными данными.</span><span class="sxs-lookup"><span data-stu-id="34de9-119">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="34de9-120">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживаются в `roleDefinitions` наборе сущностей в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="34de9-120">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="34de9-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="34de9-121">Properties</span></span>
| <span data-ttu-id="34de9-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="34de9-122">Property</span></span>          |<span data-ttu-id="34de9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="34de9-123">Type</span></span>         |<span data-ttu-id="34de9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="34de9-124">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="34de9-125">id</span><span class="sxs-lookup"><span data-stu-id="34de9-125">id</span></span>                 |<span data-ttu-id="34de9-126">String</span><span class="sxs-lookup"><span data-stu-id="34de9-126">String</span></span>     |<span data-ttu-id="34de9-127">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-127">The id of the resource.</span></span> <span data-ttu-id="34de9-128">Он указан в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="34de9-128">It is in GUID format.</span></span>|
|<span data-ttu-id="34de9-129">externalId</span><span class="sxs-lookup"><span data-stu-id="34de9-129">externalId</span></span>           |<span data-ttu-id="34de9-130">String</span><span class="sxs-lookup"><span data-stu-id="34de9-130">String</span></span>   |<span data-ttu-id="34de9-131">Внешний идентификатор ресурса, представляющий его исходный идентификатор во внешней системе.</span><span class="sxs-lookup"><span data-stu-id="34de9-131">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="34de9-132">Например, внешний идентификатор ресурса подписки может иметь значение "/Subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span><span class="sxs-lookup"><span data-stu-id="34de9-132">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="34de9-133">type</span><span class="sxs-lookup"><span data-stu-id="34de9-133">type</span></span>               |<span data-ttu-id="34de9-134">String</span><span class="sxs-lookup"><span data-stu-id="34de9-134">String</span></span>     |<span data-ttu-id="34de9-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34de9-135">Required.</span></span> <span data-ttu-id="34de9-136">Тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-136">Resource type.</span></span> <span data-ttu-id="34de9-137">Например, для ресурсов Azure типом может быть "Subscription", "ResourceGroup", "Microsoft. SQL/Server" и т. д.</span><span class="sxs-lookup"><span data-stu-id="34de9-137">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="34de9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="34de9-138">displayName</span></span>        |<span data-ttu-id="34de9-139">Строка</span><span class="sxs-lookup"><span data-stu-id="34de9-139">String</span></span>     |<span data-ttu-id="34de9-140">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-140">The display name of the resource.</span></span>|
|<span data-ttu-id="34de9-141">status</span><span class="sxs-lookup"><span data-stu-id="34de9-141">status</span></span>             |<span data-ttu-id="34de9-142">String</span><span class="sxs-lookup"><span data-stu-id="34de9-142">String</span></span>     |<span data-ttu-id="34de9-143">Состояние данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-143">The status of a given resource.</span></span> <span data-ttu-id="34de9-144">Например, он может представлять, заблокирован ли ресурс (значения: `Active` / `Locked`).</span><span class="sxs-lookup"><span data-stu-id="34de9-144">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="34de9-145">Примечание: это свойство может быть расширено в будущем для поддержки дополнительных сценариев.</span><span class="sxs-lookup"><span data-stu-id="34de9-145">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="34de9-146">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="34de9-146">registeredDateTime</span></span>|<span data-ttu-id="34de9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34de9-147">DateTimeOffset</span></span>      |<span data-ttu-id="34de9-148">Представляет дату и время, когда ресурс регистрируется в PIM.</span><span class="sxs-lookup"><span data-stu-id="34de9-148">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="34de9-149">регистередрут</span><span class="sxs-lookup"><span data-stu-id="34de9-149">registeredRoot</span></span>|<span data-ttu-id="34de9-150">String</span><span class="sxs-lookup"><span data-stu-id="34de9-150">String</span></span>      |<span data-ttu-id="34de9-151">Екстерналид из корневой области ресурса, зарегистрированной в PIM.</span><span class="sxs-lookup"><span data-stu-id="34de9-151">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="34de9-152">В качестве корневой области можно указать родительские, бабушке или более поздние ресурсы предков.</span><span class="sxs-lookup"><span data-stu-id="34de9-152">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="34de9-153">ролеассигнменткаунт</span><span class="sxs-lookup"><span data-stu-id="34de9-153">roleAssignmentCount</span></span>|<span data-ttu-id="34de9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="34de9-154">Int32</span></span>      |<span data-ttu-id="34de9-155">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="34de9-155">Optional.</span></span> <span data-ttu-id="34de9-156">Число назначений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-156">The number of role assignments for the given resource.</span></span> <span data-ttu-id="34de9-157">Чтобы получить свойство, используйте `$select=roleAssignmentCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="34de9-157">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="34de9-158">роледефинитионкаунт</span><span class="sxs-lookup"><span data-stu-id="34de9-158">roleDefinitionCount</span></span>|<span data-ttu-id="34de9-159">Int32</span><span class="sxs-lookup"><span data-stu-id="34de9-159">Int32</span></span>      |<span data-ttu-id="34de9-160">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="34de9-160">Optional.</span></span> <span data-ttu-id="34de9-161">Количество определений ролей для данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-161">The number of role definitions for the given resource.</span></span> <span data-ttu-id="34de9-162">Чтобы получить свойство, используйте `$select=roleDefinitionCount` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="34de9-162">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="34de9-163">permissions</span><span class="sxs-lookup"><span data-stu-id="34de9-163">permissions</span></span>|[<span data-ttu-id="34de9-164">governancePermission</span><span class="sxs-lookup"><span data-stu-id="34de9-164">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="34de9-165">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34de9-165">Optional.</span></span> <span data-ttu-id="34de9-166">Он представляет состояние доступа запрашивающего к ресурсу. Чтобы получить свойство, используйте `$select=permissions` експликтли в запросе.</span><span class="sxs-lookup"><span data-stu-id="34de9-166">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34de9-167">Связи</span><span class="sxs-lookup"><span data-stu-id="34de9-167">Relationships</span></span>
| <span data-ttu-id="34de9-168">Связь</span><span class="sxs-lookup"><span data-stu-id="34de9-168">Relationship</span></span>   | <span data-ttu-id="34de9-169">Тип</span><span class="sxs-lookup"><span data-stu-id="34de9-169">Type</span></span>                                         |<span data-ttu-id="34de9-170">Описание</span><span class="sxs-lookup"><span data-stu-id="34de9-170">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="34de9-171">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="34de9-171">roleAssignments</span></span> |<span data-ttu-id="34de9-172">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34de9-172">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="34de9-173">Коллекция назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-173">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="34de9-174">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="34de9-174">roleDefinitions</span></span> |<span data-ttu-id="34de9-175">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="34de9-175">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="34de9-176">Коллекция ролей дефинтионс для ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-176">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="34de9-177">ролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="34de9-177">roleAssignmentRequests</span></span> |<span data-ttu-id="34de9-178">Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="34de9-178">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="34de9-179">Коллекция запросов назначений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-179">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="34de9-180">ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="34de9-180">roleSettings</span></span> |<span data-ttu-id="34de9-181">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="34de9-181">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="34de9-182">Коллекция параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="34de9-182">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="34de9-183">верхнего</span><span class="sxs-lookup"><span data-stu-id="34de9-183">parent</span></span>          |[<span data-ttu-id="34de9-184">governanceResource</span><span class="sxs-lookup"><span data-stu-id="34de9-184">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="34de9-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34de9-185">Read-only.</span></span> <span data-ttu-id="34de9-186">Родительский ресурс.</span><span class="sxs-lookup"><span data-stu-id="34de9-186">The parent resource.</span></span> <span data-ttu-id="34de9-187">для `pimforazurerbac` сценария может представлять подписку, к которой относится ресурс.</span><span class="sxs-lookup"><span data-stu-id="34de9-187">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34de9-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34de9-188">JSON representation</span></span>

<span data-ttu-id="34de9-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34de9-189">The following is a JSON representation of the resource.</span></span>

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
