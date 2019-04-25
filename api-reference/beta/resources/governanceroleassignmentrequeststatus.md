---
title: Тип ресурса Говернанцеролеассигнментрекуестстатус
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547434"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="a67cf-103">Тип ресурса Говернанцеролеассигнментрекуестстатус</span><span class="sxs-lookup"><span data-stu-id="a67cf-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a67cf-104">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a67cf-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="a67cf-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a67cf-105">Properties</span></span>
<span data-ttu-id="a67cf-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a67cf-106">Property</span></span>       | <span data-ttu-id="a67cf-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a67cf-107">Type</span></span> |<span data-ttu-id="a67cf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a67cf-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="a67cf-109">status</span><span class="sxs-lookup"><span data-stu-id="a67cf-109">status</span></span> |<span data-ttu-id="a67cf-110">String</span><span class="sxs-lookup"><span data-stu-id="a67cf-110">String</span></span>| <span data-ttu-id="a67cf-111">Состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a67cf-111">The status of the role assignment request.</span></span> <span data-ttu-id="a67cf-112">Значение может быть `InProgress` или `Closed`.</span><span class="sxs-lookup"><span data-stu-id="a67cf-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="a67cf-113">подСостояние</span><span class="sxs-lookup"><span data-stu-id="a67cf-113">subStatus</span></span> |<span data-ttu-id="a67cf-114">String</span><span class="sxs-lookup"><span data-stu-id="a67cf-114">String</span></span>| <span data-ttu-id="a67cf-115">Дочерний статус запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a67cf-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="a67cf-116">Возможные значения `Accepted`:, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `FailedAsResourceIsLocked` `ProvisioningStarted`,,,,,,,,,,,,,, и. `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval`</span><span class="sxs-lookup"><span data-stu-id="a67cf-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="a67cf-117">Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="a67cf-117">statusDetails</span></span>       |<span data-ttu-id="a67cf-118">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a67cf-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="a67cf-119">Сведения о состоянии запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="a67cf-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="a67cf-120">Он представляет результаты оценки различных правил.</span><span class="sxs-lookup"><span data-stu-id="a67cf-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a67cf-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a67cf-121">JSON representation</span></span>

<span data-ttu-id="a67cf-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a67cf-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
