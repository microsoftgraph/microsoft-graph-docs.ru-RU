---
title: Тип ресурса dailySchedule
description: График ежедневного выполнения повторяющихся сценарий управления устройства.
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080479"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="737eb-103">Тип ресурса dailySchedule</span><span class="sxs-lookup"><span data-stu-id="737eb-103">dailySchedule resource type</span></span>

> <span data-ttu-id="737eb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="737eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="737eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="737eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="737eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="737eb-107">График ежедневного выполнения повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="737eb-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="737eb-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="737eb-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="737eb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="737eb-109">Properties</span></span>
|<span data-ttu-id="737eb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="737eb-110">Property</span></span>|<span data-ttu-id="737eb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="737eb-111">Type</span></span>|<span data-ttu-id="737eb-112">Description</span><span class="sxs-lookup"><span data-stu-id="737eb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="737eb-113">interval</span><span class="sxs-lookup"><span data-stu-id="737eb-113">interval</span></span>|<span data-ttu-id="737eb-114">Int32</span><span class="sxs-lookup"><span data-stu-id="737eb-114">Int32</span></span>|<span data-ttu-id="737eb-115">Интервал в днях</span><span class="sxs-lookup"><span data-stu-id="737eb-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="737eb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="737eb-116">Relationships</span></span>
<span data-ttu-id="737eb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="737eb-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="737eb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="737eb-118">JSON Representation</span></span>
<span data-ttu-id="737eb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="737eb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





