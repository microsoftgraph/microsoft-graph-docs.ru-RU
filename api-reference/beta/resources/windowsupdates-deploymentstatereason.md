---
title: тип ресурса deploymentStateReason
description: Причина конкретного состояния развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 19a5063cd4f103b0f065311118bc5d8ac97a3c7a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068209"
---
# <a name="deploymentstatereason-resource-type"></a><span data-ttu-id="bfa04-103">тип ресурса deploymentStateReason</span><span class="sxs-lookup"><span data-stu-id="bfa04-103">deploymentStateReason resource type</span></span>

<span data-ttu-id="bfa04-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="bfa04-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa04-105">Причина конкретного состояния развертывания.</span><span class="sxs-lookup"><span data-stu-id="bfa04-105">A reason for a particular deployment state.</span></span>

## <a name="properties"></a><span data-ttu-id="bfa04-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfa04-106">Properties</span></span>
|<span data-ttu-id="bfa04-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfa04-107">Property</span></span>|<span data-ttu-id="bfa04-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bfa04-108">Type</span></span>|<span data-ttu-id="bfa04-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bfa04-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa04-110">значение</span><span class="sxs-lookup"><span data-stu-id="bfa04-110">value</span></span>|<span data-ttu-id="bfa04-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span><span class="sxs-lookup"><span data-stu-id="bfa04-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span></span>|<span data-ttu-id="bfa04-112">Указывает причину состояния развертывания.</span><span class="sxs-lookup"><span data-stu-id="bfa04-112">Specifies a reason for the deployment state.</span></span> <span data-ttu-id="bfa04-113">Возможные значения: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`.</span><span class="sxs-lookup"><span data-stu-id="bfa04-113">Possible values are: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`.</span></span> <span data-ttu-id="bfa04-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfa04-114">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfa04-115">Связи</span><span class="sxs-lookup"><span data-stu-id="bfa04-115">Relationships</span></span>
<span data-ttu-id="bfa04-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bfa04-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfa04-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bfa04-117">JSON representation</span></span>
<span data-ttu-id="bfa04-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfa04-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentStateReason",
  "value": "String"
}
```

