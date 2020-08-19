---
title: Тип ресурса Говернанцеролеассигнментрекуестстатус
description: Представляет состояние governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: a1031429d6288ec19a9f3791e24a35dc0d431588
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809511"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="01e4e-103">Тип ресурса Говернанцеролеассигнментрекуестстатус</span><span class="sxs-lookup"><span data-stu-id="01e4e-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="01e4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01e4e-105">Представляет состояние [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="01e4e-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="01e4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="01e4e-106">Properties</span></span>
<span data-ttu-id="01e4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="01e4e-107">Property</span></span>       | <span data-ttu-id="01e4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="01e4e-108">Type</span></span> |<span data-ttu-id="01e4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="01e4e-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="01e4e-110">status</span><span class="sxs-lookup"><span data-stu-id="01e4e-110">status</span></span> |<span data-ttu-id="01e4e-111">String</span><span class="sxs-lookup"><span data-stu-id="01e4e-111">String</span></span>| <span data-ttu-id="01e4e-112">Состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="01e4e-112">The status of the role assignment request.</span></span> <span data-ttu-id="01e4e-113">Значение может быть `InProgress` или `Closed` .</span><span class="sxs-lookup"><span data-stu-id="01e4e-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="01e4e-114">подсостояние</span><span class="sxs-lookup"><span data-stu-id="01e4e-114">subStatus</span></span> |<span data-ttu-id="01e4e-115">String</span><span class="sxs-lookup"><span data-stu-id="01e4e-115">String</span></span>| <span data-ttu-id="01e4e-116">Дочерний статус запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="01e4e-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="01e4e-117">Возможные значения:,,,,,,,,,,, `Accepted` `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `PendingRevocation` `Revoked` ,,,, `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` и `ProvisioningStarted` .</span><span class="sxs-lookup"><span data-stu-id="01e4e-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="01e4e-118">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="01e4e-118">statusDetails</span></span>       |<span data-ttu-id="01e4e-119">Коллекция [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="01e4e-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="01e4e-120">Сведения о состоянии запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="01e4e-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="01e4e-121">Он представляет результаты оценки различных правил.</span><span class="sxs-lookup"><span data-stu-id="01e4e-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01e4e-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01e4e-122">JSON representation</span></span>

<span data-ttu-id="01e4e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01e4e-123">Here is a JSON representation of the resource.</span></span>

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
