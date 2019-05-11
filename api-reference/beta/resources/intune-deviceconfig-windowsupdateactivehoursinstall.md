---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49238831005d579baba2dd55e431f1ac684e67d3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943657"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="a110e-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="a110e-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="a110e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a110e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a110e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a110e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a110e-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a110e-106">Not yet documented</span></span>


<span data-ttu-id="a110e-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a110e-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a110e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a110e-108">Properties</span></span>
|<span data-ttu-id="a110e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a110e-109">Property</span></span>|<span data-ttu-id="a110e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a110e-110">Type</span></span>|<span data-ttu-id="a110e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a110e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a110e-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a110e-112">activeHoursStart</span></span>|<span data-ttu-id="a110e-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a110e-113">TimeOfDay</span></span>|<span data-ttu-id="a110e-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="a110e-114">Active Hours Start</span></span>|
|<span data-ttu-id="a110e-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a110e-115">activeHoursEnd</span></span>|<span data-ttu-id="a110e-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a110e-116">TimeOfDay</span></span>|<span data-ttu-id="a110e-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="a110e-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="a110e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a110e-118">Relationships</span></span>
<span data-ttu-id="a110e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a110e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a110e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a110e-120">JSON Representation</span></span>
<span data-ttu-id="a110e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a110e-121">Here is a JSON representation of the resource.</span></span>
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




