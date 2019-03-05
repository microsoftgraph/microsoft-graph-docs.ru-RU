---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9deab255749e70cfd165f28c27c09182b298e00a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144095"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d1805-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="d1805-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="d1805-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1805-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1805-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1805-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1805-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d1805-106">Not yet documented</span></span>


<span data-ttu-id="d1805-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d1805-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1805-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1805-108">Properties</span></span>
|<span data-ttu-id="d1805-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1805-109">Property</span></span>|<span data-ttu-id="d1805-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1805-110">Type</span></span>|<span data-ttu-id="d1805-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1805-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1805-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d1805-112">activeHoursStart</span></span>|<span data-ttu-id="d1805-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d1805-113">TimeOfDay</span></span>|<span data-ttu-id="d1805-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="d1805-114">Active Hours Start</span></span>|
|<span data-ttu-id="d1805-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d1805-115">activeHoursEnd</span></span>|<span data-ttu-id="d1805-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d1805-116">TimeOfDay</span></span>|<span data-ttu-id="d1805-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="d1805-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1805-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d1805-118">Relationships</span></span>
<span data-ttu-id="d1805-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d1805-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1805-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1805-120">JSON Representation</span></span>
<span data-ttu-id="d1805-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1805-121">Here is a JSON representation of the resource.</span></span>
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




