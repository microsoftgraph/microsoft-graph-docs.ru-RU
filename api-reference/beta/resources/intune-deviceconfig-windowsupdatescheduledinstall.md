---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 55a53c169f60361af1f695aa07452c4e4a60bedf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301647"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4c9fe-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="4c9fe-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4c9fe-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c9fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c9fe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c9fe-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4c9fe-107">Not yet documented</span></span>

<span data-ttu-id="4c9fe-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4c9fe-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c9fe-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c9fe-109">Properties</span></span>
|<span data-ttu-id="4c9fe-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c9fe-110">Property</span></span>|<span data-ttu-id="4c9fe-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4c9fe-111">Type</span></span>|<span data-ttu-id="4c9fe-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4c9fe-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c9fe-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4c9fe-113">scheduledInstallDay</span></span>|[<span data-ttu-id="4c9fe-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4c9fe-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4c9fe-115">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="4c9fe-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4c9fe-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4c9fe-117">scheduledInstallTime</span></span>|<span data-ttu-id="4c9fe-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4c9fe-118">TimeOfDay</span></span>|<span data-ttu-id="4c9fe-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="4c9fe-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c9fe-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4c9fe-120">Relationships</span></span>
<span data-ttu-id="4c9fe-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4c9fe-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c9fe-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c9fe-122">JSON Representation</span></span>
<span data-ttu-id="4c9fe-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c9fe-123">Here is a JSON representation of the resource.</span></span>
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





