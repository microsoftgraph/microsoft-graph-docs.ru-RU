---
title: Тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
ms.openlocfilehash: 06b0f17513d5d796d3fe71cbd3888963bc4a34ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076441"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="64ad2-103">Тип ресурса governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="64ad2-103">governanceRoleAssignmentRequestStatus resource type</span></span>

> <span data-ttu-id="64ad2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64ad2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64ad2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64ad2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64ad2-106">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="64ad2-106">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="64ad2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64ad2-107">Properties</span></span>
<span data-ttu-id="64ad2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="64ad2-108">Property</span></span>       | <span data-ttu-id="64ad2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="64ad2-109">Type</span></span> |<span data-ttu-id="64ad2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64ad2-110">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="64ad2-111">status</span><span class="sxs-lookup"><span data-stu-id="64ad2-111">status</span></span> |<span data-ttu-id="64ad2-112">String</span><span class="sxs-lookup"><span data-stu-id="64ad2-112">String</span></span>| <span data-ttu-id="64ad2-113">Состояние запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="64ad2-113">The status of the role assignment request.</span></span> <span data-ttu-id="64ad2-114">Значение может быть `InProgress` или `Closed`.</span><span class="sxs-lookup"><span data-stu-id="64ad2-114">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="64ad2-115">Дополнительные сведения о</span><span class="sxs-lookup"><span data-stu-id="64ad2-115">subStatus</span></span> |<span data-ttu-id="64ad2-116">String</span><span class="sxs-lookup"><span data-stu-id="64ad2-116">String</span></span>| <span data-ttu-id="64ad2-117">Состояние sub запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="64ad2-117">The sub status of the role assignment request.</span></span> <span data-ttu-id="64ad2-118">Значения могут быть `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, и `ProvisioningStarted`.</span><span class="sxs-lookup"><span data-stu-id="64ad2-118">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="64ad2-119">statusDetails</span><span class="sxs-lookup"><span data-stu-id="64ad2-119">statusDetails</span></span>       |<span data-ttu-id="64ad2-120">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="64ad2-120">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="64ad2-121">Подробные сведения о состоянии запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="64ad2-121">The details of the status of the role assignment request.</span></span> <span data-ttu-id="64ad2-122">Представляет результаты оценки различные правила.</span><span class="sxs-lookup"><span data-stu-id="64ad2-122">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64ad2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64ad2-123">JSON representation</span></span>

<span data-ttu-id="64ad2-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64ad2-124">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->