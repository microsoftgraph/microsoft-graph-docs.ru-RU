---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512929"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="393f1-103">Тип ресурса privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="393f1-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393f1-104">Представляет группу функциональные возможности службы управления правами Identity (PIM).</span><span class="sxs-lookup"><span data-stu-id="393f1-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="393f1-105">Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="393f1-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="393f1-106">`privilegedAccess`доступно только для чтения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="393f1-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="393f1-107">Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.</span><span class="sxs-lookup"><span data-stu-id="393f1-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="393f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="393f1-108">Properties</span></span>
| <span data-ttu-id="393f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="393f1-109">Property</span></span>  | <span data-ttu-id="393f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="393f1-110">Type</span></span>      |<span data-ttu-id="393f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="393f1-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="393f1-112">id</span><span class="sxs-lookup"><span data-stu-id="393f1-112">id</span></span>         |<span data-ttu-id="393f1-113">String</span><span class="sxs-lookup"><span data-stu-id="393f1-113">String</span></span>     |<span data-ttu-id="393f1-114">Идентификатор поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="393f1-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="393f1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="393f1-115">displayName</span></span>|<span data-ttu-id="393f1-116">String</span><span class="sxs-lookup"><span data-stu-id="393f1-116">String</span></span>     |<span data-ttu-id="393f1-117">Отображаемое имя поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="393f1-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="393f1-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="393f1-118">Relationships</span></span>
| <span data-ttu-id="393f1-119">Связь</span><span class="sxs-lookup"><span data-stu-id="393f1-119">Relationship</span></span>   | <span data-ttu-id="393f1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="393f1-120">Type</span></span>                                         |<span data-ttu-id="393f1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="393f1-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="393f1-122">resources</span><span class="sxs-lookup"><span data-stu-id="393f1-122">resources</span></span>       |<span data-ttu-id="393f1-123">[governanceResource](../resources/governanceresource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="393f1-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="393f1-124">Набор ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="393f1-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="393f1-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="393f1-125">roleAssignments</span></span> |<span data-ttu-id="393f1-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="393f1-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="393f1-127">Коллекция назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="393f1-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="393f1-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="393f1-128">roleDefinitions</span></span> |<span data-ttu-id="393f1-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="393f1-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="393f1-130">Коллекция файлов определения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="393f1-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="393f1-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="393f1-131">roleAssignmentRequests</span></span> |<span data-ttu-id="393f1-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="393f1-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="393f1-133">Коллекция запросы назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="393f1-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="393f1-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="393f1-134">roleSettings</span></span> |<span data-ttu-id="393f1-135">[governanceRoleSetting](../resources/governancerolesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="393f1-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="393f1-136">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="393f1-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="393f1-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="393f1-137">JSON representation</span></span>

<span data-ttu-id="393f1-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="393f1-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
