---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3635441f015d49ffb402f5314896e9e68b15e8e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030928"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d1f5a-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="d1f5a-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="d1f5a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1f5a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f5a-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d1f5a-105">Not yet documented</span></span>


<span data-ttu-id="d1f5a-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5a-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1f5a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1f5a-107">Properties</span></span>
|<span data-ttu-id="d1f5a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f5a-108">Property</span></span>|<span data-ttu-id="d1f5a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f5a-109">Type</span></span>|<span data-ttu-id="d1f5a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f5a-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d1f5a-111">activeHoursStart</span></span>|<span data-ttu-id="d1f5a-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d1f5a-112">TimeOfDay</span></span>|<span data-ttu-id="d1f5a-113">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="d1f5a-113">Active Hours Start</span></span>|
|<span data-ttu-id="d1f5a-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d1f5a-114">activeHoursEnd</span></span>|<span data-ttu-id="d1f5a-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d1f5a-115">TimeOfDay</span></span>|<span data-ttu-id="d1f5a-116">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="d1f5a-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1f5a-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1f5a-117">Relationships</span></span>
<span data-ttu-id="d1f5a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f5a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1f5a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1f5a-119">JSON Representation</span></span>
<span data-ttu-id="d1f5a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1f5a-120">Here is a JSON representation of the resource.</span></span>
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



