---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19e0ced371108103398e26c6067f4ce3b3ab67e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806407"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6113e-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="6113e-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="6113e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6113e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6113e-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6113e-105">Not yet documented</span></span>

<span data-ttu-id="6113e-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6113e-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6113e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6113e-107">Properties</span></span>
|<span data-ttu-id="6113e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6113e-108">Property</span></span>|<span data-ttu-id="6113e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6113e-109">Type</span></span>|<span data-ttu-id="6113e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6113e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6113e-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6113e-111">scheduledInstallDay</span></span>|[<span data-ttu-id="6113e-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="6113e-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6113e-113">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="6113e-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="6113e-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6113e-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6113e-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6113e-115">scheduledInstallTime</span></span>|<span data-ttu-id="6113e-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6113e-116">TimeOfDay</span></span>|<span data-ttu-id="6113e-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="6113e-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6113e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="6113e-118">Relationships</span></span>
<span data-ttu-id="6113e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6113e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6113e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6113e-120">JSON Representation</span></span>
<span data-ttu-id="6113e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6113e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



