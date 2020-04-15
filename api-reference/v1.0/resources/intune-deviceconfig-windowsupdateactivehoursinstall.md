---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 124ac24616ee8662bd0224fd2a063e523dfdb260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451401"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="04aa4-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="04aa4-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="04aa4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04aa4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04aa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04aa4-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04aa4-106">Not yet documented</span></span>


<span data-ttu-id="04aa4-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="04aa4-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04aa4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04aa4-108">Properties</span></span>
|<span data-ttu-id="04aa4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04aa4-109">Property</span></span>|<span data-ttu-id="04aa4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04aa4-110">Type</span></span>|<span data-ttu-id="04aa4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04aa4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04aa4-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="04aa4-112">activeHoursStart</span></span>|<span data-ttu-id="04aa4-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="04aa4-113">TimeOfDay</span></span>|<span data-ttu-id="04aa4-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="04aa4-114">Active Hours Start</span></span>|
|<span data-ttu-id="04aa4-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="04aa4-115">activeHoursEnd</span></span>|<span data-ttu-id="04aa4-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="04aa4-116">TimeOfDay</span></span>|<span data-ttu-id="04aa4-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="04aa4-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="04aa4-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="04aa4-118">Relationships</span></span>
<span data-ttu-id="04aa4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="04aa4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04aa4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04aa4-120">JSON Representation</span></span>
<span data-ttu-id="04aa4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04aa4-121">Here is a JSON representation of the resource.</span></span>
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







