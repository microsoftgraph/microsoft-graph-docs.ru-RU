---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad513d4022b991917a7afe8ce9bdf012095621de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931246"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="606c8-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="606c8-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="606c8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="606c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="606c8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="606c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="606c8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="606c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="606c8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="606c8-107">Not yet documented</span></span>

<span data-ttu-id="606c8-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="606c8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="606c8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="606c8-109">Properties</span></span>
|<span data-ttu-id="606c8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="606c8-110">Property</span></span>|<span data-ttu-id="606c8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="606c8-111">Type</span></span>|<span data-ttu-id="606c8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="606c8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="606c8-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="606c8-113">activeHoursStart</span></span>|<span data-ttu-id="606c8-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="606c8-114">TimeOfDay</span></span>|<span data-ttu-id="606c8-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="606c8-115">Active Hours Start</span></span>|
|<span data-ttu-id="606c8-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="606c8-116">activeHoursEnd</span></span>|<span data-ttu-id="606c8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="606c8-117">TimeOfDay</span></span>|<span data-ttu-id="606c8-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="606c8-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="606c8-119">Связи</span><span class="sxs-lookup"><span data-stu-id="606c8-119">Relationships</span></span>
<span data-ttu-id="606c8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="606c8-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="606c8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="606c8-121">JSON Representation</span></span>
<span data-ttu-id="606c8-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="606c8-122">Here is a JSON representation of the resource.</span></span>
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





