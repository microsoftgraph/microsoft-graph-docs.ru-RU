---
title: Тип ресурса Привилежедакцесс
description: " Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1c8388c8ba9fd79b44e0d037496313cf67774bdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521560"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="f375c-103">Тип ресурса Привилежедакцесс</span><span class="sxs-lookup"><span data-stu-id="f375c-103">privilegedAccess resource type</span></span>

<span data-ttu-id="f375c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f375c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f375c-105">Представляет группу функциональных возможностей, предоставляемых службой управления привилегированными удостоверениями (PIM).</span><span class="sxs-lookup"><span data-stu-id="f375c-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="f375c-106">Различные экземпляры `privilegedAccess` представляют разных поставщиков, УПРАВЛЯЕМЫХ службой PIM; Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="f375c-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="f375c-107">`privilegedAccess`в настоящее время доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f375c-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="f375c-108">`PUT` `POST` `privilegedAccess` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH`</span><span class="sxs-lookup"><span data-stu-id="f375c-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="f375c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f375c-109">Properties</span></span>
| <span data-ttu-id="f375c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f375c-110">Property</span></span>  | <span data-ttu-id="f375c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f375c-111">Type</span></span>      |<span data-ttu-id="f375c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f375c-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="f375c-113">id</span><span class="sxs-lookup"><span data-stu-id="f375c-113">id</span></span>         |<span data-ttu-id="f375c-114">String</span><span class="sxs-lookup"><span data-stu-id="f375c-114">String</span></span>     |<span data-ttu-id="f375c-115">Идентификатор поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="f375c-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="f375c-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f375c-116">displayName</span></span>|<span data-ttu-id="f375c-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f375c-117">String</span></span>     |<span data-ttu-id="f375c-118">Отображаемое имя поставщика, управляемого службой PIM.</span><span class="sxs-lookup"><span data-stu-id="f375c-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f375c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f375c-119">Relationships</span></span>
| <span data-ttu-id="f375c-120">Связь</span><span class="sxs-lookup"><span data-stu-id="f375c-120">Relationship</span></span>   | <span data-ttu-id="f375c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f375c-121">Type</span></span>                                         |<span data-ttu-id="f375c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f375c-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="f375c-123">resources</span><span class="sxs-lookup"><span data-stu-id="f375c-123">resources</span></span>       |<span data-ttu-id="f375c-124">Коллекция [governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="f375c-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="f375c-125">Коллекция ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f375c-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="f375c-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="f375c-126">roleAssignments</span></span> |<span data-ttu-id="f375c-127">Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f375c-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="f375c-128">Коллекция назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f375c-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="f375c-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f375c-129">roleDefinitions</span></span> |<span data-ttu-id="f375c-130">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f375c-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="f375c-131">Коллекция ролей дефинтионс для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f375c-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="f375c-132">ролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="f375c-132">roleAssignmentRequests</span></span> |<span data-ttu-id="f375c-133">Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f375c-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="f375c-134">Коллекция запросов назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f375c-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="f375c-135">ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="f375c-135">roleSettings</span></span> |<span data-ttu-id="f375c-136">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f375c-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="f375c-137">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f375c-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f375c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f375c-138">JSON representation</span></span>

<span data-ttu-id="f375c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f375c-139">Here is a JSON representation of the resource.</span></span>

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
