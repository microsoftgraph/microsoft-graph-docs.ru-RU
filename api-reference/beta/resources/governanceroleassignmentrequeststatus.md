---
title: Тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510178"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="8e36e-103">Тип ресурса governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="8e36e-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e36e-104">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="8e36e-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="8e36e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e36e-105">Properties</span></span>
<span data-ttu-id="8e36e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e36e-106">Property</span></span>       | <span data-ttu-id="8e36e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8e36e-107">Type</span></span> |<span data-ttu-id="8e36e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8e36e-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="8e36e-109">status</span><span class="sxs-lookup"><span data-stu-id="8e36e-109">status</span></span> |<span data-ttu-id="8e36e-110">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-110">String</span></span>| <span data-ttu-id="8e36e-111">Состояние запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8e36e-111">The status of the role assignment request.</span></span> <span data-ttu-id="8e36e-112">Значение может быть `InProgress` или `Closed`.</span><span class="sxs-lookup"><span data-stu-id="8e36e-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="8e36e-113">Дополнительные сведения о</span><span class="sxs-lookup"><span data-stu-id="8e36e-113">subStatus</span></span> |<span data-ttu-id="8e36e-114">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-114">String</span></span>| <span data-ttu-id="8e36e-115">Состояние sub запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8e36e-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="8e36e-116">Значения могут быть `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, и `ProvisioningStarted`.</span><span class="sxs-lookup"><span data-stu-id="8e36e-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="8e36e-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="8e36e-117">statusDetails</span></span>       |<span data-ttu-id="8e36e-118">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8e36e-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="8e36e-119">Подробные сведения о состоянии запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8e36e-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="8e36e-120">Представляет результаты оценки различные правила.</span><span class="sxs-lookup"><span data-stu-id="8e36e-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e36e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e36e-121">JSON representation</span></span>

<span data-ttu-id="8e36e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e36e-122">Here is a JSON representation of the resource.</span></span>

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
