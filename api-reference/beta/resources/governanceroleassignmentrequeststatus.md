---
title: Тип ресурса Говернанцеролеассигнментрекуестстатус
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 287f9f6ab7b1442ebdd517edbb27175fc36e6108
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497407"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="81d3a-103">Тип ресурса Говернанцеролеассигнментрекуестстатус</span><span class="sxs-lookup"><span data-stu-id="81d3a-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="81d3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81d3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81d3a-105">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="81d3a-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="81d3a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="81d3a-106">Properties</span></span>
<span data-ttu-id="81d3a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="81d3a-107">Property</span></span>       | <span data-ttu-id="81d3a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="81d3a-108">Type</span></span> |<span data-ttu-id="81d3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="81d3a-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="81d3a-110">status</span><span class="sxs-lookup"><span data-stu-id="81d3a-110">status</span></span> |<span data-ttu-id="81d3a-111">String</span><span class="sxs-lookup"><span data-stu-id="81d3a-111">String</span></span>| <span data-ttu-id="81d3a-112">Состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="81d3a-112">The status of the role assignment request.</span></span> <span data-ttu-id="81d3a-113">Значение может быть `InProgress` или `Closed`.</span><span class="sxs-lookup"><span data-stu-id="81d3a-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="81d3a-114">подсостояние</span><span class="sxs-lookup"><span data-stu-id="81d3a-114">subStatus</span></span> |<span data-ttu-id="81d3a-115">String</span><span class="sxs-lookup"><span data-stu-id="81d3a-115">String</span></span>| <span data-ttu-id="81d3a-116">Дочерний статус запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="81d3a-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="81d3a-117">Возможные значения `Accepted`:, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `FailedAsResourceIsLocked` `ProvisioningStarted`,,,,,,,,,,,,,, и. `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval`</span><span class="sxs-lookup"><span data-stu-id="81d3a-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="81d3a-118">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="81d3a-118">statusDetails</span></span>       |<span data-ttu-id="81d3a-119">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="81d3a-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="81d3a-120">Сведения о состоянии запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="81d3a-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="81d3a-121">Он представляет результаты оценки различных правил.</span><span class="sxs-lookup"><span data-stu-id="81d3a-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81d3a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81d3a-122">JSON representation</span></span>

<span data-ttu-id="81d3a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81d3a-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
