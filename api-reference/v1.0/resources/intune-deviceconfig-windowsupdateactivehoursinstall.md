---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 556e0f22bb249a8606b3bbf9bb3252d3721793b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845740"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="424dc-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="424dc-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="424dc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="424dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="424dc-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="424dc-105">Not yet documented</span></span>

<span data-ttu-id="424dc-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="424dc-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="424dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="424dc-107">Properties</span></span>
|<span data-ttu-id="424dc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="424dc-108">Property</span></span>|<span data-ttu-id="424dc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="424dc-109">Type</span></span>|<span data-ttu-id="424dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="424dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="424dc-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="424dc-111">activeHoursStart</span></span>|<span data-ttu-id="424dc-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="424dc-112">TimeOfDay</span></span>|<span data-ttu-id="424dc-113">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="424dc-113">Active Hours Start</span></span>|
|<span data-ttu-id="424dc-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="424dc-114">activeHoursEnd</span></span>|<span data-ttu-id="424dc-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="424dc-115">TimeOfDay</span></span>|<span data-ttu-id="424dc-116">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="424dc-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="424dc-117">Связи</span><span class="sxs-lookup"><span data-stu-id="424dc-117">Relationships</span></span>
<span data-ttu-id="424dc-118">Нет</span><span class="sxs-lookup"><span data-stu-id="424dc-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="424dc-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="424dc-119">JSON Representation</span></span>
<span data-ttu-id="424dc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="424dc-120">Here is a JSON representation of the resource.</span></span>
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



