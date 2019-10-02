---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29b885bcfd728f412d2e94ecdbdbdfc23ee9fb76
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357166"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="4592c-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="4592c-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="4592c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4592c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4592c-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4592c-105">Not yet documented</span></span>


<span data-ttu-id="4592c-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4592c-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4592c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4592c-107">Properties</span></span>
|<span data-ttu-id="4592c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4592c-108">Property</span></span>|<span data-ttu-id="4592c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4592c-109">Type</span></span>|<span data-ttu-id="4592c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4592c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4592c-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="4592c-111">activeHoursStart</span></span>|<span data-ttu-id="4592c-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4592c-112">TimeOfDay</span></span>|<span data-ttu-id="4592c-113">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="4592c-113">Active Hours Start</span></span>|
|<span data-ttu-id="4592c-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="4592c-114">activeHoursEnd</span></span>|<span data-ttu-id="4592c-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4592c-115">TimeOfDay</span></span>|<span data-ttu-id="4592c-116">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="4592c-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="4592c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="4592c-117">Relationships</span></span>
<span data-ttu-id="4592c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4592c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4592c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4592c-119">JSON Representation</span></span>
<span data-ttu-id="4592c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4592c-120">Here is a JSON representation of the resource.</span></span>
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




