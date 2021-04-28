---
title: тип ресурса deploymentState
description: Описывает текущее состояние развертывания и контролирует его.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067487"
---
# <a name="deploymentstate-resource-type"></a><span data-ttu-id="1d97a-103">тип ресурса deploymentState</span><span class="sxs-lookup"><span data-stu-id="1d97a-103">deploymentState resource type</span></span>

<span data-ttu-id="1d97a-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1d97a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d97a-105">Описывает текущее состояние развертывания и контролирует его.</span><span class="sxs-lookup"><span data-stu-id="1d97a-105">Describes and controls the current state of a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="1d97a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d97a-106">Properties</span></span>
|<span data-ttu-id="1d97a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d97a-107">Property</span></span>|<span data-ttu-id="1d97a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1d97a-108">Type</span></span>|<span data-ttu-id="1d97a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1d97a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d97a-110">причины</span><span class="sxs-lookup"><span data-stu-id="1d97a-110">reasons</span></span>|<span data-ttu-id="1d97a-111">[коллекция microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)</span><span class="sxs-lookup"><span data-stu-id="1d97a-111">[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) collection</span></span>|<span data-ttu-id="1d97a-112">Указывает причины, по которой развертывание имеет свое значение состояния.</span><span class="sxs-lookup"><span data-stu-id="1d97a-112">Specifies the reasons the deployment has its state value.</span></span> <span data-ttu-id="1d97a-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d97a-113">Read-only.</span></span>|
|<span data-ttu-id="1d97a-114">requestedValue</span><span class="sxs-lookup"><span data-stu-id="1d97a-114">requestedValue</span></span>|<span data-ttu-id="1d97a-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="1d97a-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span></span>|<span data-ttu-id="1d97a-116">Указывает запрашиваемого состояния развертывания.</span><span class="sxs-lookup"><span data-stu-id="1d97a-116">Specifies the requested state of the deployment.</span></span> <span data-ttu-id="1d97a-117">Поддерживает подмножество значений **для запрашиваемогоDeploymentStateValue.**</span><span class="sxs-lookup"><span data-stu-id="1d97a-117">Supports a subset of the values for **requestedDeploymentStateValue**.</span></span> <span data-ttu-id="1d97a-118">Возможные значения: `none`, `paused`.</span><span class="sxs-lookup"><span data-stu-id="1d97a-118">Possible values are: `none`, `paused`.</span></span>|
|<span data-ttu-id="1d97a-119">значение</span><span class="sxs-lookup"><span data-stu-id="1d97a-119">value</span></span>|<span data-ttu-id="1d97a-120">microsoft.graph.windowsUpdates.deploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="1d97a-120">microsoft.graph.windowsUpdates.deploymentStateValue</span></span>|<span data-ttu-id="1d97a-121">Указывает состояние развертывания.</span><span class="sxs-lookup"><span data-stu-id="1d97a-121">Specifies the state of the deployment.</span></span> <span data-ttu-id="1d97a-122">Поддерживает подмножество значений **для deploymentStateValue.**</span><span class="sxs-lookup"><span data-stu-id="1d97a-122">Supports a subset of the values for **deploymentStateValue**.</span></span> <span data-ttu-id="1d97a-123">Возможные значения: `scheduled`, `offering`, `paused`.</span><span class="sxs-lookup"><span data-stu-id="1d97a-123">Possible values are: `scheduled`, `offering`, `paused`.</span></span> <span data-ttu-id="1d97a-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d97a-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d97a-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1d97a-125">Relationships</span></span>
<span data-ttu-id="1d97a-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1d97a-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d97a-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1d97a-127">JSON representation</span></span>
<span data-ttu-id="1d97a-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d97a-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

