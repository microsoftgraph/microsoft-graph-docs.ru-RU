---
title: Тип ресурса hourlySchedule
description: Каждый час запустите расписание для повторяющихся сценарий управления устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004481786fd21ad04e0adbe4e16d3174fc6cc2f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951889"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="c979d-103">Тип ресурса hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="c979d-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="c979d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c979d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c979d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c979d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c979d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c979d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c979d-107">Каждый час запустите расписание для повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="c979d-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="c979d-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c979d-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c979d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c979d-109">Properties</span></span>
|<span data-ttu-id="c979d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c979d-110">Property</span></span>|<span data-ttu-id="c979d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c979d-111">Type</span></span>|<span data-ttu-id="c979d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c979d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c979d-113">interval</span><span class="sxs-lookup"><span data-stu-id="c979d-113">interval</span></span>|<span data-ttu-id="c979d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c979d-114">Int32</span></span>|<span data-ttu-id="c979d-115">Интервал в часах</span><span class="sxs-lookup"><span data-stu-id="c979d-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="c979d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c979d-116">Relationships</span></span>
<span data-ttu-id="c979d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c979d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c979d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c979d-118">JSON Representation</span></span>
<span data-ttu-id="c979d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c979d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```





