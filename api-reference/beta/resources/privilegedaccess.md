---
title: Тип ресурса privilegedAccess
description: " например, `privilegedAccess/azureResources` представляет PIM, управляющее привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a144ba13974a728b4e89fc661f34f20e8157689
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136621"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="31d63-103">Тип ресурса privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="31d63-103">privilegedAccess resource type</span></span>

<span data-ttu-id="31d63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31d63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31d63-105">Представляет группу функций, предоставляемых службой Privileged Identity Management (PIM).</span><span class="sxs-lookup"><span data-stu-id="31d63-105">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="31d63-106">Разные экземпляры представляют различных поставщиков, управляемых `privilegedAccess` PIM; например, представляет PIM, управляющую привилегированным доступом `privilegedAccess/azureResources` к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="31d63-106">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="31d63-107">`privilegedAccess` в настоящее время находится только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31d63-107">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="31d63-108">Нет, не поддерживаются операции или `POST` операции для `PUT` набора `PATCH` `DELETE` `privilegedAccess` суностей.</span><span class="sxs-lookup"><span data-stu-id="31d63-108">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="31d63-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31d63-109">Properties</span></span>
| <span data-ttu-id="31d63-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31d63-110">Property</span></span>  | <span data-ttu-id="31d63-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31d63-111">Type</span></span>      |<span data-ttu-id="31d63-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31d63-112">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="31d63-113">id</span><span class="sxs-lookup"><span data-stu-id="31d63-113">id</span></span>         |<span data-ttu-id="31d63-114">Строка</span><span class="sxs-lookup"><span data-stu-id="31d63-114">String</span></span>     |<span data-ttu-id="31d63-115">ИД поставщика, управляемого PIM.</span><span class="sxs-lookup"><span data-stu-id="31d63-115">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="31d63-116">displayName</span><span class="sxs-lookup"><span data-stu-id="31d63-116">displayName</span></span>|<span data-ttu-id="31d63-117">Строка</span><span class="sxs-lookup"><span data-stu-id="31d63-117">String</span></span>     |<span data-ttu-id="31d63-118">Отображаемого имени поставщика, управляемого PIM.</span><span class="sxs-lookup"><span data-stu-id="31d63-118">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="31d63-119">Связи</span><span class="sxs-lookup"><span data-stu-id="31d63-119">Relationships</span></span>
| <span data-ttu-id="31d63-120">Связь</span><span class="sxs-lookup"><span data-stu-id="31d63-120">Relationship</span></span>   | <span data-ttu-id="31d63-121">Тип</span><span class="sxs-lookup"><span data-stu-id="31d63-121">Type</span></span>                                         |<span data-ttu-id="31d63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31d63-122">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="31d63-123">resources</span><span class="sxs-lookup"><span data-stu-id="31d63-123">resources</span></span>       |<span data-ttu-id="31d63-124">[коллекция governanceResource](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="31d63-124">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="31d63-125">Коллекция ресурсов для поставщика.</span><span class="sxs-lookup"><span data-stu-id="31d63-125">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="31d63-126">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="31d63-126">roleAssignments</span></span> |<span data-ttu-id="31d63-127">[Коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="31d63-127">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="31d63-128">Коллекция назначений ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="31d63-128">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="31d63-129">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="31d63-129">roleDefinitions</span></span> |<span data-ttu-id="31d63-130">[Коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31d63-130">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="31d63-131">Коллекция отозванных ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="31d63-131">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="31d63-132">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="31d63-132">roleAssignmentRequests</span></span> |<span data-ttu-id="31d63-133">[Коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="31d63-133">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="31d63-134">Коллекция запросов на назначение ролей для поставщика.</span><span class="sxs-lookup"><span data-stu-id="31d63-134">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="31d63-135">roleSettings</span><span class="sxs-lookup"><span data-stu-id="31d63-135">roleSettings</span></span> |<span data-ttu-id="31d63-136">[Коллекция governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="31d63-136">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="31d63-137">Коллекция параметров роли для поставщика.</span><span class="sxs-lookup"><span data-stu-id="31d63-137">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="31d63-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31d63-138">JSON representation</span></span>

<span data-ttu-id="31d63-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31d63-139">Here is a JSON representation of the resource.</span></span>

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


