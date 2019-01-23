---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28f40501123f465d8fcbfa05c3febb8ffab6f27a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409470"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="71b15-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="71b15-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="71b15-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71b15-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71b15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71b15-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71b15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b15-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="71b15-107">Not yet documented</span></span>


<span data-ttu-id="71b15-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="71b15-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71b15-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="71b15-109">Properties</span></span>
|<span data-ttu-id="71b15-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="71b15-110">Property</span></span>|<span data-ttu-id="71b15-111">Тип</span><span class="sxs-lookup"><span data-stu-id="71b15-111">Type</span></span>|<span data-ttu-id="71b15-112">Описание</span><span class="sxs-lookup"><span data-stu-id="71b15-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b15-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="71b15-113">activeHoursStart</span></span>|<span data-ttu-id="71b15-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="71b15-114">TimeOfDay</span></span>|<span data-ttu-id="71b15-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="71b15-115">Active Hours Start</span></span>|
|<span data-ttu-id="71b15-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="71b15-116">activeHoursEnd</span></span>|<span data-ttu-id="71b15-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="71b15-117">TimeOfDay</span></span>|<span data-ttu-id="71b15-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="71b15-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="71b15-119">Связи</span><span class="sxs-lookup"><span data-stu-id="71b15-119">Relationships</span></span>
<span data-ttu-id="71b15-120">Нет</span><span class="sxs-lookup"><span data-stu-id="71b15-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71b15-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71b15-121">JSON Representation</span></span>
<span data-ttu-id="71b15-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71b15-122">Here is a JSON representation of the resource.</span></span>
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




