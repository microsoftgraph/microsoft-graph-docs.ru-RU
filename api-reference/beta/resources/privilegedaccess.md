---
title: Тип ресурса Привилежедакцесс
description: " Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7f59f8420be6ff97511415e944d154cb5d59950f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965791"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="c2eb0-103">Тип ресурса Привилежедакцесс</span><span class="sxs-lookup"><span data-stu-id="c2eb0-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2eb0-104">Представляет группу функциональных возможностей, предоставляемых службой управления привилегированными удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="c2eb0-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="c2eb0-105">Различные экземпляры `privilegedAccess` представляют разных поставщиков, УПРАВЛЯЕМЫХ службой PIM; Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="c2eb0-106">`privilegedAccess`в настоящее время доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="c2eb0-107">`PUT` `POST` `privilegedAccess` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH`</span><span class="sxs-lookup"><span data-stu-id="c2eb0-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="c2eb0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2eb0-108">Properties</span></span>
| <span data-ttu-id="c2eb0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2eb0-109">Property</span></span>  | <span data-ttu-id="c2eb0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2eb0-110">Type</span></span>      |<span data-ttu-id="c2eb0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2eb0-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="c2eb0-112">id</span><span class="sxs-lookup"><span data-stu-id="c2eb0-112">id</span></span>         |<span data-ttu-id="c2eb0-113">String</span><span class="sxs-lookup"><span data-stu-id="c2eb0-113">String</span></span>     |<span data-ttu-id="c2eb0-114">Идентификатор поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="c2eb0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c2eb0-115">displayName</span></span>|<span data-ttu-id="c2eb0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="c2eb0-116">String</span></span>     |<span data-ttu-id="c2eb0-117">Отображаемое имя поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c2eb0-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="c2eb0-118">Relationships</span></span>
| <span data-ttu-id="c2eb0-119">Отношение</span><span class="sxs-lookup"><span data-stu-id="c2eb0-119">Relationship</span></span>   | <span data-ttu-id="c2eb0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c2eb0-120">Type</span></span>                                         |<span data-ttu-id="c2eb0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2eb0-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="c2eb0-122">resources</span><span class="sxs-lookup"><span data-stu-id="c2eb0-122">resources</span></span>       |<span data-ttu-id="c2eb0-123">Коллекция [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb0-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="c2eb0-124">Коллекция ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="c2eb0-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c2eb0-125">roleAssignments</span></span> |<span data-ttu-id="c2eb0-126">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb0-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="c2eb0-127">Коллекция назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="c2eb0-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c2eb0-128">roleDefinitions</span></span> |<span data-ttu-id="c2eb0-129">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb0-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="c2eb0-130">Коллекция ролей дефинтионс для поставщика.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="c2eb0-131">Ролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="c2eb0-131">roleAssignmentRequests</span></span> |<span data-ttu-id="c2eb0-132">Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb0-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="c2eb0-133">Коллекция запросов назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="c2eb0-134">Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="c2eb0-134">roleSettings</span></span> |<span data-ttu-id="c2eb0-135">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb0-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="c2eb0-136">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c2eb0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2eb0-137">JSON representation</span></span>

<span data-ttu-id="c2eb0-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2eb0-138">Here is a JSON representation of the resource.</span></span>

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
