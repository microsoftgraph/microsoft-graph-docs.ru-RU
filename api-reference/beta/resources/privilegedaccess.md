---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082437"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="a36a1-103">Тип ресурса privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="a36a1-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="a36a1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a36a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a36a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a36a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a36a1-106">Представляет группу функциональные возможности службы управления правами Identity (PIM).</span><span class="sxs-lookup"><span data-stu-id="a36a1-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="a36a1-107">Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="a36a1-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="a36a1-108">`privilegedAccess`доступно только для чтения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="a36a1-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="a36a1-109">Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.</span><span class="sxs-lookup"><span data-stu-id="a36a1-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="a36a1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="a36a1-110">Properties</span></span>
| <span data-ttu-id="a36a1-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="a36a1-111">Property</span></span>  | <span data-ttu-id="a36a1-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a36a1-112">Type</span></span>      |<span data-ttu-id="a36a1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a36a1-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a36a1-114">id</span><span class="sxs-lookup"><span data-stu-id="a36a1-114">id</span></span>         |<span data-ttu-id="a36a1-115">String</span><span class="sxs-lookup"><span data-stu-id="a36a1-115">String</span></span>     |<span data-ttu-id="a36a1-116">Идентификатор поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="a36a1-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="a36a1-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a36a1-117">displayName</span></span>|<span data-ttu-id="a36a1-118">String</span><span class="sxs-lookup"><span data-stu-id="a36a1-118">String</span></span>     |<span data-ttu-id="a36a1-119">Отображаемое имя поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="a36a1-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a36a1-120">Связи</span><span class="sxs-lookup"><span data-stu-id="a36a1-120">Relationships</span></span>
| <span data-ttu-id="a36a1-121">Связь</span><span class="sxs-lookup"><span data-stu-id="a36a1-121">Relationship</span></span>   | <span data-ttu-id="a36a1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a36a1-122">Type</span></span>                                         |<span data-ttu-id="a36a1-123">Description</span><span class="sxs-lookup"><span data-stu-id="a36a1-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="a36a1-124">resources</span><span class="sxs-lookup"><span data-stu-id="a36a1-124">resources</span></span>       |<span data-ttu-id="a36a1-125">[governanceResource](../resources/governanceresource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a36a1-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="a36a1-126">Набор ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="a36a1-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="a36a1-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a36a1-127">roleAssignments</span></span> |<span data-ttu-id="a36a1-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a36a1-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="a36a1-129">Коллекция назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="a36a1-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="a36a1-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a36a1-130">roleDefinitions</span></span> |<span data-ttu-id="a36a1-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a36a1-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="a36a1-132">Коллекция файлов определения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="a36a1-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="a36a1-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a36a1-133">roleAssignmentRequests</span></span> |<span data-ttu-id="a36a1-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a36a1-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="a36a1-135">Коллекция запросы назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="a36a1-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="a36a1-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="a36a1-136">roleSettings</span></span> |<span data-ttu-id="a36a1-137">[governanceRoleSetting](../resources/governancerolesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a36a1-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="a36a1-138">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="a36a1-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a36a1-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a36a1-139">JSON representation</span></span>

<span data-ttu-id="a36a1-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a36a1-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
