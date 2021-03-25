---
title: тип ресурса userExperienceAnalyticsAutopilotDevicesSummary
description: Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159468"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a><span data-ttu-id="6b730-103">тип ресурса userExperienceAnalyticsAutopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="6b730-103">userExperienceAnalyticsAutopilotDevicesSummary resource type</span></span>

<span data-ttu-id="6b730-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b730-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b730-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b730-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b730-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b730-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b730-107">Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.</span><span class="sxs-lookup"><span data-stu-id="6b730-107">The user experience analytics summary of Devices not windows autopilot ready.</span></span>

## <a name="properties"></a><span data-ttu-id="6b730-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b730-108">Properties</span></span>
|<span data-ttu-id="6b730-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b730-109">Property</span></span>|<span data-ttu-id="6b730-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6b730-110">Type</span></span>|<span data-ttu-id="6b730-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b730-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b730-112">devicesNotAutopilotRegistered</span><span class="sxs-lookup"><span data-stu-id="6b730-112">devicesNotAutopilotRegistered</span></span>|<span data-ttu-id="6b730-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6b730-113">Int32</span></span>|<span data-ttu-id="6b730-114">Количество устройств intune, которые не зарегистрированы автопилотом.</span><span class="sxs-lookup"><span data-stu-id="6b730-114">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="6b730-115">devicesWithoutAutopilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="6b730-115">devicesWithoutAutopilotProfileAssigned</span></span>|<span data-ttu-id="6b730-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6b730-116">Int32</span></span>|<span data-ttu-id="6b730-117">Количество устройств intune, не назначенное профилем автопилота.</span><span class="sxs-lookup"><span data-stu-id="6b730-117">The count of intune devices not autopilot profile assigned.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b730-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="6b730-118">Relationships</span></span>
<span data-ttu-id="6b730-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6b730-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b730-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b730-120">JSON Representation</span></span>
<span data-ttu-id="6b730-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b730-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




