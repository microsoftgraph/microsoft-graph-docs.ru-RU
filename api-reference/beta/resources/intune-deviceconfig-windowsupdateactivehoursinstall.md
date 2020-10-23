---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67c6ec798df120f9c7c14fbf2392450d05bb8afb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695014"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="24454-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="24454-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="24454-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24454-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24454-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24454-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24454-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24454-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24454-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="24454-107">Not yet documented</span></span>


<span data-ttu-id="24454-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="24454-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24454-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24454-109">Properties</span></span>
|<span data-ttu-id="24454-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24454-110">Property</span></span>|<span data-ttu-id="24454-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24454-111">Type</span></span>|<span data-ttu-id="24454-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24454-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24454-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="24454-113">activeHoursStart</span></span>|<span data-ttu-id="24454-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="24454-114">TimeOfDay</span></span>|<span data-ttu-id="24454-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="24454-115">Active Hours Start</span></span>|
|<span data-ttu-id="24454-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="24454-116">activeHoursEnd</span></span>|<span data-ttu-id="24454-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="24454-117">TimeOfDay</span></span>|<span data-ttu-id="24454-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="24454-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="24454-119">Связи</span><span class="sxs-lookup"><span data-stu-id="24454-119">Relationships</span></span>
<span data-ttu-id="24454-120">Нет</span><span class="sxs-lookup"><span data-stu-id="24454-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24454-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24454-121">JSON Representation</span></span>
<span data-ttu-id="24454-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24454-122">Here is a JSON representation of the resource.</span></span>
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





