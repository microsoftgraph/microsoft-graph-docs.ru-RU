---
title: Тип ресурса Говернанцеролеассигнментрекуестстатус
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 768ef092dbe52b0989277905bae03eee091ca8c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340327"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="f0582-103">Тип ресурса Говернанцеролеассигнментрекуестстатус</span><span class="sxs-lookup"><span data-stu-id="f0582-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0582-104">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f0582-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="f0582-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0582-105">Properties</span></span>
<span data-ttu-id="f0582-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0582-106">Property</span></span>       | <span data-ttu-id="f0582-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f0582-107">Type</span></span> |<span data-ttu-id="f0582-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f0582-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="f0582-109">status</span><span class="sxs-lookup"><span data-stu-id="f0582-109">status</span></span> |<span data-ttu-id="f0582-110">String</span><span class="sxs-lookup"><span data-stu-id="f0582-110">String</span></span>| <span data-ttu-id="f0582-111">Состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f0582-111">The status of the role assignment request.</span></span> <span data-ttu-id="f0582-112">Значение может быть `InProgress` или `Closed`.</span><span class="sxs-lookup"><span data-stu-id="f0582-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="f0582-113">подСостояние</span><span class="sxs-lookup"><span data-stu-id="f0582-113">subStatus</span></span> |<span data-ttu-id="f0582-114">String</span><span class="sxs-lookup"><span data-stu-id="f0582-114">String</span></span>| <span data-ttu-id="f0582-115">Дочерний статус запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f0582-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="f0582-116">Возможные значения `Accepted`:, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `FailedAsResourceIsLocked` `ProvisioningStarted`,,,,,,,,,,,,,, и. `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval`</span><span class="sxs-lookup"><span data-stu-id="f0582-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="f0582-117">Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="f0582-117">statusDetails</span></span>       |<span data-ttu-id="f0582-118">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f0582-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="f0582-119">Сведения о состоянии запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f0582-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="f0582-120">Он представляет результаты оценки различных правил.</span><span class="sxs-lookup"><span data-stu-id="f0582-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0582-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0582-121">JSON representation</span></span>

<span data-ttu-id="f0582-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0582-122">Here is a JSON representation of the resource.</span></span>

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
