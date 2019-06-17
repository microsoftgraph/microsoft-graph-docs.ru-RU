---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0c40fc7ade30a73212d1917294671fdb5423483
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978768"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="f3c5a-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="f3c5a-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="f3c5a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3c5a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3c5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c5a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f3c5a-106">Not yet documented</span></span>


<span data-ttu-id="f3c5a-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="f3c5a-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3c5a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3c5a-108">Properties</span></span>
|<span data-ttu-id="f3c5a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3c5a-109">Property</span></span>|<span data-ttu-id="f3c5a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3c5a-110">Type</span></span>|<span data-ttu-id="f3c5a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c5a-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="f3c5a-112">activeHoursStart</span></span>|<span data-ttu-id="f3c5a-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3c5a-113">TimeOfDay</span></span>|<span data-ttu-id="f3c5a-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="f3c5a-114">Active Hours Start</span></span>|
|<span data-ttu-id="f3c5a-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="f3c5a-115">activeHoursEnd</span></span>|<span data-ttu-id="f3c5a-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3c5a-116">TimeOfDay</span></span>|<span data-ttu-id="f3c5a-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="f3c5a-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3c5a-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3c5a-118">Relationships</span></span>
<span data-ttu-id="f3c5a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f3c5a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3c5a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3c5a-120">JSON Representation</span></span>
<span data-ttu-id="f3c5a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3c5a-121">Here is a JSON representation of the resource.</span></span>
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





