---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8621b0fecbb8960843173195845287445fb3686
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786209"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="35988-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="35988-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="35988-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35988-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35988-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35988-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35988-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="35988-106">Not yet documented</span></span>


<span data-ttu-id="35988-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="35988-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35988-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35988-108">Properties</span></span>
|<span data-ttu-id="35988-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35988-109">Property</span></span>|<span data-ttu-id="35988-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35988-110">Type</span></span>|<span data-ttu-id="35988-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35988-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35988-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="35988-112">activeHoursStart</span></span>|<span data-ttu-id="35988-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="35988-113">TimeOfDay</span></span>|<span data-ttu-id="35988-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="35988-114">Active Hours Start</span></span>|
|<span data-ttu-id="35988-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="35988-115">activeHoursEnd</span></span>|<span data-ttu-id="35988-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="35988-116">TimeOfDay</span></span>|<span data-ttu-id="35988-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="35988-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="35988-118">Связи</span><span class="sxs-lookup"><span data-stu-id="35988-118">Relationships</span></span>
<span data-ttu-id="35988-119">Нет</span><span class="sxs-lookup"><span data-stu-id="35988-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35988-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35988-120">JSON Representation</span></span>
<span data-ttu-id="35988-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35988-121">Here is a JSON representation of the resource.</span></span>
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



