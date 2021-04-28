---
title: тип ресурса monitoringRule
description: Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068088"
---
# <a name="monitoringrule-resource-type"></a><span data-ttu-id="80743-103">тип ресурса monitoringRule</span><span class="sxs-lookup"><span data-stu-id="80743-103">monitoringRule resource type</span></span>

<span data-ttu-id="80743-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="80743-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80743-105">Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.</span><span class="sxs-lookup"><span data-stu-id="80743-105">Rule defining a signal and threshold to monitor, and the action to perform when met.</span></span>

## <a name="properties"></a><span data-ttu-id="80743-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="80743-106">Properties</span></span>
|<span data-ttu-id="80743-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="80743-107">Property</span></span>|<span data-ttu-id="80743-108">Тип</span><span class="sxs-lookup"><span data-stu-id="80743-108">Type</span></span>|<span data-ttu-id="80743-109">Описание</span><span class="sxs-lookup"><span data-stu-id="80743-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80743-110">action</span><span class="sxs-lookup"><span data-stu-id="80743-110">action</span></span>|<span data-ttu-id="80743-111">microsoft.graph.windowsUpdates.monitoringAction</span><span class="sxs-lookup"><span data-stu-id="80743-111">microsoft.graph.windowsUpdates.monitoringAction</span></span>|    <span data-ttu-id="80743-112">Действие, срабатывае при превышении порогового значения для данного сигнала.</span><span class="sxs-lookup"><span data-stu-id="80743-112">The action triggered when the threshold for the given signal is met.</span></span> <span data-ttu-id="80743-113">Возможные значения: `alertError`, `pauseDeployment`.</span><span class="sxs-lookup"><span data-stu-id="80743-113">Possible values are: `alertError`, `pauseDeployment`.</span></span>|
|<span data-ttu-id="80743-114">сигнал</span><span class="sxs-lookup"><span data-stu-id="80743-114">signal</span></span>|<span data-ttu-id="80743-115">microsoft.graph.windowsUpdates.monitoringSignal</span><span class="sxs-lookup"><span data-stu-id="80743-115">microsoft.graph.windowsUpdates.monitoringSignal</span></span>|<span data-ttu-id="80743-116">Сигнал для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="80743-116">The signal to monitor.</span></span> <span data-ttu-id="80743-117">Возможные значения: `rollback` .</span><span class="sxs-lookup"><span data-stu-id="80743-117">Possible values are: `rollback`.</span></span>|
|<span data-ttu-id="80743-118">пороговое значение</span><span class="sxs-lookup"><span data-stu-id="80743-118">threshold</span></span>|<span data-ttu-id="80743-119">Int32</span><span class="sxs-lookup"><span data-stu-id="80743-119">Int32</span></span>|<span data-ttu-id="80743-120">Пороговое значение для сигнала, с которого можно запускать действие.</span><span class="sxs-lookup"><span data-stu-id="80743-120">The threshold for a signal at which to trigger action.</span></span> <span data-ttu-id="80743-121">Включительно от 1 до 100 ( включительно).</span><span class="sxs-lookup"><span data-stu-id="80743-121">An integer from 1 to 100 (inclusive).</span></span>|

## <a name="relationships"></a><span data-ttu-id="80743-122">Связи</span><span class="sxs-lookup"><span data-stu-id="80743-122">Relationships</span></span>
<span data-ttu-id="80743-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80743-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80743-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="80743-124">JSON representation</span></span>
<span data-ttu-id="80743-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80743-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

