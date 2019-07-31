---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d6534e859be60a9fe0cf921e46eefb88bca0282
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968696"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="da62b-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="da62b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="da62b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da62b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da62b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da62b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da62b-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="da62b-106">Not yet documented</span></span>


<span data-ttu-id="da62b-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="da62b-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da62b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da62b-108">Properties</span></span>
|<span data-ttu-id="da62b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da62b-109">Property</span></span>|<span data-ttu-id="da62b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da62b-110">Type</span></span>|<span data-ttu-id="da62b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da62b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da62b-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="da62b-112">activeHoursStart</span></span>|<span data-ttu-id="da62b-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="da62b-113">TimeOfDay</span></span>|<span data-ttu-id="da62b-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="da62b-114">Active Hours Start</span></span>|
|<span data-ttu-id="da62b-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="da62b-115">activeHoursEnd</span></span>|<span data-ttu-id="da62b-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="da62b-116">TimeOfDay</span></span>|<span data-ttu-id="da62b-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="da62b-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="da62b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="da62b-118">Relationships</span></span>
<span data-ttu-id="da62b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="da62b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da62b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da62b-120">JSON Representation</span></span>
<span data-ttu-id="da62b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da62b-121">Here is a JSON representation of the resource.</span></span>
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





