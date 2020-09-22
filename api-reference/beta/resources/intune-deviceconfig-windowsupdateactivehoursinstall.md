---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ae015503909ff6b9c627923ff809cebaa91468d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039701"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="6328a-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="6328a-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="6328a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6328a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6328a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6328a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6328a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6328a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6328a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6328a-107">Not yet documented</span></span>


<span data-ttu-id="6328a-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6328a-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6328a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6328a-109">Properties</span></span>
|<span data-ttu-id="6328a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6328a-110">Property</span></span>|<span data-ttu-id="6328a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6328a-111">Type</span></span>|<span data-ttu-id="6328a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6328a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6328a-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6328a-113">activeHoursStart</span></span>|<span data-ttu-id="6328a-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6328a-114">TimeOfDay</span></span>|<span data-ttu-id="6328a-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="6328a-115">Active Hours Start</span></span>|
|<span data-ttu-id="6328a-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6328a-116">activeHoursEnd</span></span>|<span data-ttu-id="6328a-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6328a-117">TimeOfDay</span></span>|<span data-ttu-id="6328a-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="6328a-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="6328a-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="6328a-119">Relationships</span></span>
<span data-ttu-id="6328a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6328a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6328a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6328a-121">JSON Representation</span></span>
<span data-ttu-id="6328a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6328a-122">Here is a JSON representation of the resource.</span></span>
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






