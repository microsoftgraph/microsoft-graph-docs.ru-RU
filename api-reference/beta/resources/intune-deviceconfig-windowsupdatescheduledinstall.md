---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae4cb747cb4648cd9f4cc9550933688d180dd38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952043"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="091d8-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="091d8-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="091d8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="091d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="091d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="091d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="091d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="091d8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="091d8-107">Not yet documented</span></span>

<span data-ttu-id="091d8-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="091d8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="091d8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="091d8-109">Properties</span></span>
|<span data-ttu-id="091d8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="091d8-110">Property</span></span>|<span data-ttu-id="091d8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="091d8-111">Type</span></span>|<span data-ttu-id="091d8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="091d8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="091d8-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="091d8-113">scheduledInstallDay</span></span>|[<span data-ttu-id="091d8-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="091d8-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="091d8-115">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="091d8-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="091d8-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="091d8-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="091d8-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="091d8-117">scheduledInstallTime</span></span>|<span data-ttu-id="091d8-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="091d8-118">TimeOfDay</span></span>|<span data-ttu-id="091d8-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="091d8-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="091d8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="091d8-120">Relationships</span></span>
<span data-ttu-id="091d8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="091d8-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="091d8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="091d8-122">JSON Representation</span></span>
<span data-ttu-id="091d8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="091d8-123">Here is a JSON representation of the resource.</span></span>
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





