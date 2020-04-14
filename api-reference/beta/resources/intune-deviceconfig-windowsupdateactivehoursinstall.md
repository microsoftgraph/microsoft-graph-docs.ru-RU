---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5e9b8f4f55f2709fe5db513e801937e05e0f38a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453428"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="3a1a9-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="3a1a9-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="3a1a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a1a9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a1a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a1a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a1a9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3a1a9-107">Not yet documented</span></span>


<span data-ttu-id="3a1a9-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="3a1a9-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a1a9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a1a9-109">Properties</span></span>
|<span data-ttu-id="3a1a9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a1a9-110">Property</span></span>|<span data-ttu-id="3a1a9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3a1a9-111">Type</span></span>|<span data-ttu-id="3a1a9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3a1a9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a1a9-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="3a1a9-113">activeHoursStart</span></span>|<span data-ttu-id="3a1a9-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3a1a9-114">TimeOfDay</span></span>|<span data-ttu-id="3a1a9-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="3a1a9-115">Active Hours Start</span></span>|
|<span data-ttu-id="3a1a9-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="3a1a9-116">activeHoursEnd</span></span>|<span data-ttu-id="3a1a9-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3a1a9-117">TimeOfDay</span></span>|<span data-ttu-id="3a1a9-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="3a1a9-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a1a9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="3a1a9-119">Relationships</span></span>
<span data-ttu-id="3a1a9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3a1a9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a1a9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a1a9-121">JSON Representation</span></span>
<span data-ttu-id="3a1a9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a1a9-122">Here is a JSON representation of the resource.</span></span>
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



