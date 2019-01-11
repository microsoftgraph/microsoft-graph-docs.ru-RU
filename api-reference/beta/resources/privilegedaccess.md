---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810054"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="4914e-103">Тип ресурса privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="4914e-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="4914e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4914e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4914e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4914e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4914e-106">Представляет группу функциональные возможности службы управления правами Identity (PIM).</span><span class="sxs-lookup"><span data-stu-id="4914e-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="4914e-107">Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="4914e-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="4914e-108">`privilegedAccess`доступно только для чтения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="4914e-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="4914e-109">Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.</span><span class="sxs-lookup"><span data-stu-id="4914e-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="4914e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4914e-110">Properties</span></span>
| <span data-ttu-id="4914e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="4914e-111">Property</span></span>  | <span data-ttu-id="4914e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4914e-112">Type</span></span>      |<span data-ttu-id="4914e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4914e-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4914e-114">id</span><span class="sxs-lookup"><span data-stu-id="4914e-114">id</span></span>         |<span data-ttu-id="4914e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4914e-115">String</span></span>     |<span data-ttu-id="4914e-116">Идентификатор поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="4914e-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="4914e-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4914e-117">displayName</span></span>|<span data-ttu-id="4914e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4914e-118">String</span></span>     |<span data-ttu-id="4914e-119">Отображаемое имя поставщика, управляется PIM.</span><span class="sxs-lookup"><span data-stu-id="4914e-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4914e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4914e-120">Relationships</span></span>
| <span data-ttu-id="4914e-121">Связь</span><span class="sxs-lookup"><span data-stu-id="4914e-121">Relationship</span></span>   | <span data-ttu-id="4914e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4914e-122">Type</span></span>                                         |<span data-ttu-id="4914e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4914e-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="4914e-124">resources</span><span class="sxs-lookup"><span data-stu-id="4914e-124">resources</span></span>       |<span data-ttu-id="4914e-125">[governanceResource](../resources/governanceresource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4914e-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="4914e-126">Набор ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="4914e-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="4914e-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="4914e-127">roleAssignments</span></span> |<span data-ttu-id="4914e-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4914e-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="4914e-129">Коллекция назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="4914e-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="4914e-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="4914e-130">roleDefinitions</span></span> |<span data-ttu-id="4914e-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4914e-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="4914e-132">Коллекция файлов определения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="4914e-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="4914e-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4914e-133">roleAssignmentRequests</span></span> |<span data-ttu-id="4914e-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4914e-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="4914e-135">Коллекция запросы назначения ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="4914e-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="4914e-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="4914e-136">roleSettings</span></span> |<span data-ttu-id="4914e-137">[governanceRoleSetting](../resources/governancerolesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4914e-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="4914e-138">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="4914e-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4914e-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4914e-139">JSON representation</span></span>

<span data-ttu-id="4914e-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4914e-140">Here is a JSON representation of the resource.</span></span>

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
