---
title: тип ресурса cloudPcProvisioningPolicyAssignment
description: Назначения политики подготовка CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a96c3717b97b3f721c77b1150841f1eb51ded89f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082246"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="5f1d2-103">тип ресурса cloudPcProvisioningPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5f1d2-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="5f1d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f1d2-105">Представляет определенный набор назначений политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="5f1d2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f1d2-106">Properties</span></span>

|<span data-ttu-id="5f1d2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f1d2-107">Property</span></span>|<span data-ttu-id="5f1d2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5f1d2-108">Type</span></span>|<span data-ttu-id="5f1d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1d2-110">id</span><span class="sxs-lookup"><span data-stu-id="5f1d2-110">id</span></span>|<span data-ttu-id="5f1d2-111">String</span><span class="sxs-lookup"><span data-stu-id="5f1d2-111">String</span></span>|<span data-ttu-id="5f1d2-112">Уникальный идентификатор для назначения политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="5f1d2-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-113">Read-only.</span></span> <span data-ttu-id="5f1d2-114">Если это группа пользователей, то ID отображается как `target` {policyId} \_ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-114">If `target` is a user group, then the ID is shown as {policyId}\_{groupId}.</span></span>|
|<span data-ttu-id="5f1d2-115">target</span><span class="sxs-lookup"><span data-stu-id="5f1d2-115">target</span></span>|[<span data-ttu-id="5f1d2-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5f1d2-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="5f1d2-117">Цель назначения для политики обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="5f1d2-118">В настоящее время единственной целью, поддерживаемой для этой политики, является группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-118">Currently, the only target supported for this policy is a user group.</span></span> <span data-ttu-id="5f1d2-119">Подробные сведения см. [в материале cloudPcManagementGroupAssignmentTarget.](cloudpcmanagementgroupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5f1d2-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f1d2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5f1d2-120">Relationships</span></span>

<span data-ttu-id="5f1d2-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f1d2-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5f1d2-122">JSON representation</span></span>

<span data-ttu-id="5f1d2-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1d2-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
