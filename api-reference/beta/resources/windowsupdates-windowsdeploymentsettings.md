---
title: тип ресурса windowsDeploymentSettings
description: Параметры, когда и как служба развертывает Windows 10 обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bc55f0643e789c802254064797bf8a5c2047cb64
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067496"
---
# <a name="windowsdeploymentsettings-resource-type"></a><span data-ttu-id="d8461-103">тип ресурса windowsDeploymentSettings</span><span class="sxs-lookup"><span data-stu-id="d8461-103">windowsDeploymentSettings resource type</span></span>

<span data-ttu-id="d8461-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d8461-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8461-105">Параметры, когда и как служба развертывает Windows 10 обновления.</span><span class="sxs-lookup"><span data-stu-id="d8461-105">Settings controlling when and how the service deploys a Windows 10 update.</span></span>

<span data-ttu-id="d8461-106">Наследует [от deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d8461-106">Inherits from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8461-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8461-107">Properties</span></span>
|<span data-ttu-id="d8461-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8461-108">Property</span></span>|<span data-ttu-id="d8461-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d8461-109">Type</span></span>|<span data-ttu-id="d8461-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8461-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8461-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="d8461-111">monitoring</span></span>|[<span data-ttu-id="d8461-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="d8461-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="d8461-113">Параметры для мониторинга и автоматизации действий.</span><span class="sxs-lookup"><span data-stu-id="d8461-113">Settings governing conditions to monitor and automated actions to take.</span></span> <span data-ttu-id="d8461-114">Наследуется [от deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d8461-114">Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="d8461-115">выкатка</span><span class="sxs-lookup"><span data-stu-id="d8461-115">rollout</span></span>|[<span data-ttu-id="d8461-116">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="d8461-116">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="d8461-117">Параметры, как выкатываются материалы. Наследуется [от deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d8461-117">Settings governing how the content is rolled out. Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="d8461-118">userExperience</span><span class="sxs-lookup"><span data-stu-id="d8461-118">userExperience</span></span>|[<span data-ttu-id="d8461-119">microsoft.graph.windowsUpdates.userExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="d8461-119">microsoft.graph.windowsUpdates.userExperienceSettings</span></span>](../resources/windowsupdates-userexperiencesettings.md)|<span data-ttu-id="d8461-120">Параметры управлять опытом обновления пользователя на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d8461-120">Settings governing the user's update experience on a device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8461-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d8461-121">Relationships</span></span>
<span data-ttu-id="d8461-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8461-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8461-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d8461-123">JSON representation</span></span>
<span data-ttu-id="d8461-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8461-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsDeploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "userExperience": {
    "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
  }
}
```

