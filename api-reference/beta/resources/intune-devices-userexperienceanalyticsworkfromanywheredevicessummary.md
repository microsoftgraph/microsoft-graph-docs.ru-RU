---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: Аналитика пользовательского интерфейса Work From Anywhere metrics devices summary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6448bbc89ebe8357fa14a375f82fb73938f6634
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146800"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a><span data-ttu-id="ffa1d-103">тип ресурса userExperienceAnalyticsWorkFromAnywhereDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-103">userExperienceAnalyticsWorkFromAnywhereDevicesSummary resource type</span></span>

<span data-ttu-id="ffa1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffa1d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffa1d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffa1d-107">Аналитика пользовательского интерфейса Work From Anywhere metrics devices summary.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-107">The user experience analytics Work From Anywhere metrics devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="ffa1d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffa1d-108">Properties</span></span>
|<span data-ttu-id="ffa1d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffa1d-109">Property</span></span>|<span data-ttu-id="ffa1d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ffa1d-110">Type</span></span>|<span data-ttu-id="ffa1d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffa1d-112">autopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-112">autopilotDevicesSummary</span></span>|[<span data-ttu-id="ffa1d-113">userExperienceAnalyticsAutopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-113">userExperienceAnalyticsAutopilotDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|<span data-ttu-id="ffa1d-114">Значение работы из любого сводки устройств автопилота.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-114">The value of work from anywhere autopilot devices summary.</span></span>|
|<span data-ttu-id="ffa1d-115">cloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-115">cloudManagementDevicesSummary</span></span>|[<span data-ttu-id="ffa1d-116">userExperienceAnalyticsCloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-116">userExperienceAnalyticsCloudManagementDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|<span data-ttu-id="ffa1d-117">Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-117">The user experience work from anywhere Cloud management devices summary.</span></span>|
|<span data-ttu-id="ffa1d-118">windows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-118">windows10DevicesSummary</span></span>|[<span data-ttu-id="ffa1d-119">userExperienceAnalyticsWindows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="ffa1d-119">userExperienceAnalyticsWindows10DevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|<span data-ttu-id="ffa1d-120">Аналитика пользовательских интерфейсов работает из любого сводки устройств Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-120">The user experience analytics work from anywhere Windows 10 devices summary.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffa1d-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="ffa1d-121">Relationships</span></span>
<span data-ttu-id="ffa1d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ffa1d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffa1d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffa1d-123">JSON Representation</span></span>
<span data-ttu-id="ffa1d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffa1d-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
  "autopilotDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
    "devicesNotAutopilotRegistered": 1024,
    "devicesWithoutAutopilotProfileAssigned": 1024
  },
  "cloudManagementDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
    "coManagedDeviceCount": 1024,
    "intuneDeviceCount": 1024,
    "tenantAttachDeviceCount": 1024
  },
  "windows10DevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
    "unsupportedOSversionDeviceCount": 1024
  }
}
```




