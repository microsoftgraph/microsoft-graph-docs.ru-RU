---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d9460051726b93f61d10a2f9127bdaada76d397
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091462"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="73ba2-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="73ba2-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="73ba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73ba2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73ba2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73ba2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73ba2-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="73ba2-106">Not yet documented</span></span>


<span data-ttu-id="73ba2-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="73ba2-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73ba2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="73ba2-108">Properties</span></span>
|<span data-ttu-id="73ba2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="73ba2-109">Property</span></span>|<span data-ttu-id="73ba2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="73ba2-110">Type</span></span>|<span data-ttu-id="73ba2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="73ba2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ba2-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="73ba2-112">activeHoursStart</span></span>|<span data-ttu-id="73ba2-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="73ba2-113">TimeOfDay</span></span>|<span data-ttu-id="73ba2-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="73ba2-114">Active Hours Start</span></span>|
|<span data-ttu-id="73ba2-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="73ba2-115">activeHoursEnd</span></span>|<span data-ttu-id="73ba2-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="73ba2-116">TimeOfDay</span></span>|<span data-ttu-id="73ba2-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="73ba2-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="73ba2-118">Связи</span><span class="sxs-lookup"><span data-stu-id="73ba2-118">Relationships</span></span>
<span data-ttu-id="73ba2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="73ba2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73ba2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73ba2-120">JSON Representation</span></span>
<span data-ttu-id="73ba2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73ba2-121">Here is a JSON representation of the resource.</span></span>
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









