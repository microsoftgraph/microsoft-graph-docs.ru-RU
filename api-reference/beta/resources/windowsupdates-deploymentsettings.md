---
title: тип ресурса deploymentSettings
description: Параметры, когда и как служба развертывает обновление.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f7c00ec8e880e7fd7ae9109fd1ac015868da902a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068093"
---
# <a name="deploymentsettings-resource-type"></a><span data-ttu-id="3adeb-103">тип ресурса deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="3adeb-103">deploymentSettings resource type</span></span>

<span data-ttu-id="3adeb-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3adeb-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3adeb-105">Параметры, когда и как служба развертывает обновление.</span><span class="sxs-lookup"><span data-stu-id="3adeb-105">Settings controlling when and how the service deploys an update.</span></span>

<span data-ttu-id="3adeb-106">Базовый тип [windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3adeb-106">Base type of [windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3adeb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3adeb-107">Properties</span></span>
|<span data-ttu-id="3adeb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3adeb-108">Property</span></span>|<span data-ttu-id="3adeb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3adeb-109">Type</span></span>|<span data-ttu-id="3adeb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3adeb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3adeb-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="3adeb-111">monitoring</span></span>|[<span data-ttu-id="3adeb-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="3adeb-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="3adeb-113">Параметры для мониторинга и автоматизации действий.</span><span class="sxs-lookup"><span data-stu-id="3adeb-113">Settings governing conditions to monitor and automated actions to take.</span></span>|
|<span data-ttu-id="3adeb-114">выкатка</span><span class="sxs-lookup"><span data-stu-id="3adeb-114">rollout</span></span>|[<span data-ttu-id="3adeb-115">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="3adeb-115">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="3adeb-116">Параметры, как выкатываются материалы.</span><span class="sxs-lookup"><span data-stu-id="3adeb-116">Settings governing how the content is rolled out.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3adeb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="3adeb-117">Relationships</span></span>
<span data-ttu-id="3adeb-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3adeb-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3adeb-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3adeb-119">JSON representation</span></span>
<span data-ttu-id="3adeb-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3adeb-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  }
}
```

