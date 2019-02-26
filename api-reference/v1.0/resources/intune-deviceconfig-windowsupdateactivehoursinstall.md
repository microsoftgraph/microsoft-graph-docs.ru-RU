---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264059"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="def4f-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="def4f-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="def4f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="def4f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def4f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="def4f-105">Not yet documented</span></span>


<span data-ttu-id="def4f-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="def4f-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="def4f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="def4f-107">Properties</span></span>
|<span data-ttu-id="def4f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="def4f-108">Property</span></span>|<span data-ttu-id="def4f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="def4f-109">Type</span></span>|<span data-ttu-id="def4f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="def4f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def4f-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="def4f-111">activeHoursStart</span></span>|<span data-ttu-id="def4f-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="def4f-112">TimeOfDay</span></span>|<span data-ttu-id="def4f-113">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="def4f-113">Active Hours Start</span></span>|
|<span data-ttu-id="def4f-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="def4f-114">activeHoursEnd</span></span>|<span data-ttu-id="def4f-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="def4f-115">TimeOfDay</span></span>|<span data-ttu-id="def4f-116">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="def4f-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="def4f-117">Связи</span><span class="sxs-lookup"><span data-stu-id="def4f-117">Relationships</span></span>
<span data-ttu-id="def4f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="def4f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="def4f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="def4f-119">JSON Representation</span></span>
<span data-ttu-id="def4f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def4f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



