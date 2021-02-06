---
title: Тип ресурса governanceRoleAssignmentRequestStatus
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 99fc5ef72c40a5eff30a5e33ed89316e56c26962
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128612"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="cb2e9-103">Тип ресурса governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="cb2e9-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="cb2e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb2e9-105">Представляет состояние [governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="cb2e9-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="cb2e9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb2e9-106">Properties</span></span>
<span data-ttu-id="cb2e9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb2e9-107">Property</span></span>       | <span data-ttu-id="cb2e9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb2e9-108">Type</span></span> |<span data-ttu-id="cb2e9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2e9-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="cb2e9-110">status</span><span class="sxs-lookup"><span data-stu-id="cb2e9-110">status</span></span> |<span data-ttu-id="cb2e9-111">String</span><span class="sxs-lookup"><span data-stu-id="cb2e9-111">String</span></span>| <span data-ttu-id="cb2e9-112">Состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="cb2e9-112">The status of the role assignment request.</span></span> <span data-ttu-id="cb2e9-113">Значение может быть `InProgress` или `Closed` .</span><span class="sxs-lookup"><span data-stu-id="cb2e9-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="cb2e9-114">subStatus</span><span class="sxs-lookup"><span data-stu-id="cb2e9-114">subStatus</span></span> |<span data-ttu-id="cb2e9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="cb2e9-115">String</span></span>| <span data-ttu-id="cb2e9-116">Под состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="cb2e9-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="cb2e9-117">Значения: , `Accepted` `PendingEvaluation` , `Granted` , , , `Denied` , , , , , , `PendingProvisioning` , , , , , `Provisioned` , , `PendingRevocation` `Revoked` и `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` .</span><span class="sxs-lookup"><span data-stu-id="cb2e9-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="cb2e9-118">statusDetails</span><span class="sxs-lookup"><span data-stu-id="cb2e9-118">statusDetails</span></span>       |<span data-ttu-id="cb2e9-119">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cb2e9-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="cb2e9-120">Сведения о состоянии запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="cb2e9-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="cb2e9-121">Он представляет результаты оценки различных правил.</span><span class="sxs-lookup"><span data-stu-id="cb2e9-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb2e9-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cb2e9-122">JSON representation</span></span>

<span data-ttu-id="cb2e9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb2e9-123">Here is a JSON representation of the resource.</span></span>

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


