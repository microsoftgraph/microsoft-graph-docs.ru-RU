---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a3164a11c940538bc6ffc67ac4b1911df85f27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525392"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="6da80-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="6da80-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="6da80-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6da80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6da80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6da80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da80-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6da80-107">Not yet documented</span></span>


<span data-ttu-id="6da80-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6da80-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6da80-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6da80-109">Properties</span></span>
|<span data-ttu-id="6da80-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da80-110">Property</span></span>|<span data-ttu-id="6da80-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6da80-111">Type</span></span>|<span data-ttu-id="6da80-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6da80-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da80-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6da80-113">activeHoursStart</span></span>|<span data-ttu-id="6da80-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6da80-114">TimeOfDay</span></span>|<span data-ttu-id="6da80-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="6da80-115">Active Hours Start</span></span>|
|<span data-ttu-id="6da80-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6da80-116">activeHoursEnd</span></span>|<span data-ttu-id="6da80-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6da80-117">TimeOfDay</span></span>|<span data-ttu-id="6da80-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="6da80-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da80-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6da80-119">Relationships</span></span>
<span data-ttu-id="6da80-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6da80-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6da80-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6da80-121">JSON Representation</span></span>
<span data-ttu-id="6da80-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da80-122">Here is a JSON representation of the resource.</span></span>
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



