---
title: Тип ресурса Привилежедакцесс
description: " Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: c57dd911d105ba4d096a09f9262b847db5240fa1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811454"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="62182-103">Тип ресурса Привилежедакцесс</span><span class="sxs-lookup"><span data-stu-id="62182-103">privilegedAccess resource type</span></span>

<span data-ttu-id="62182-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62182-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62182-105">Представляет группу функциональных возможностей, предоставляемых службой управления привилегированными удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="62182-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="62182-106">Различные экземпляры `privilegedAccess` представляют разных поставщиков, УПРАВЛЯЕМЫХ PIM; например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="62182-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="62182-107">`privilegedAccess` в настоящее время доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62182-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="62182-108">`POST` `PUT` `PATCH` `DELETE` В наборе сущностей поддерживаются не поддерживаемые операции, а также операции `privilegedAccess` .</span><span class="sxs-lookup"><span data-stu-id="62182-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="62182-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="62182-109">Properties</span></span>
| <span data-ttu-id="62182-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="62182-110">Property</span></span>  | <span data-ttu-id="62182-111">Тип</span><span class="sxs-lookup"><span data-stu-id="62182-111">Type</span></span>      |<span data-ttu-id="62182-112">Описание</span><span class="sxs-lookup"><span data-stu-id="62182-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="62182-113">id</span><span class="sxs-lookup"><span data-stu-id="62182-113">id</span></span>         |<span data-ttu-id="62182-114">String</span><span class="sxs-lookup"><span data-stu-id="62182-114">String</span></span>     |<span data-ttu-id="62182-115">Идентификатор поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="62182-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="62182-116">displayName</span><span class="sxs-lookup"><span data-stu-id="62182-116">displayName</span></span>|<span data-ttu-id="62182-117">String</span><span class="sxs-lookup"><span data-stu-id="62182-117">String</span></span>     |<span data-ttu-id="62182-118">Отображаемое имя поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="62182-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="62182-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="62182-119">Relationships</span></span>
| <span data-ttu-id="62182-120">Связь</span><span class="sxs-lookup"><span data-stu-id="62182-120">Relationship</span></span>   | <span data-ttu-id="62182-121">Тип</span><span class="sxs-lookup"><span data-stu-id="62182-121">Type</span></span>                                         |<span data-ttu-id="62182-122">Описание</span><span class="sxs-lookup"><span data-stu-id="62182-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="62182-123">resources</span><span class="sxs-lookup"><span data-stu-id="62182-123">resources</span></span>       |<span data-ttu-id="62182-124">Коллекция [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="62182-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="62182-125">Коллекция ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="62182-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="62182-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="62182-126">roleAssignments</span></span> |<span data-ttu-id="62182-127">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="62182-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="62182-128">Коллекция назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="62182-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="62182-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="62182-129">roleDefinitions</span></span> |<span data-ttu-id="62182-130">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62182-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="62182-131">Коллекция ролей дефинтионс для поставщика.</span><span class="sxs-lookup"><span data-stu-id="62182-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="62182-132">ролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="62182-132">roleAssignmentRequests</span></span> |<span data-ttu-id="62182-133">Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="62182-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="62182-134">Коллекция запросов назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="62182-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="62182-135">ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="62182-135">roleSettings</span></span> |<span data-ttu-id="62182-136">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="62182-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="62182-137">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="62182-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="62182-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="62182-138">JSON representation</span></span>

<span data-ttu-id="62182-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62182-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
