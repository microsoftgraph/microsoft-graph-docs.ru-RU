---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f4089132a9ba98152fab645537dd5f835282ddb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735983"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="00655-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="00655-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="00655-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00655-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00655-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00655-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00655-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00655-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="00655-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="00655-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00655-108">Properties</span></span>
|<span data-ttu-id="00655-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00655-109">Property</span></span>|<span data-ttu-id="00655-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00655-110">Type</span></span>|<span data-ttu-id="00655-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00655-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00655-112">type</span><span class="sxs-lookup"><span data-stu-id="00655-112">type</span></span>|[<span data-ttu-id="00655-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="00655-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="00655-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="00655-114">Device type.</span></span> <span data-ttu-id="00655-115">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="00655-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="00655-116">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="00655-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="00655-117">Строка</span><span class="sxs-lookup"><span data-stu-id="00655-117">String</span></span>|<span data-ttu-id="00655-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="00655-118">Minimum OS version</span></span>|
|<span data-ttu-id="00655-119">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="00655-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="00655-120">Строка</span><span class="sxs-lookup"><span data-stu-id="00655-120">String</span></span>|<span data-ttu-id="00655-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="00655-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="00655-122">Связи</span><span class="sxs-lookup"><span data-stu-id="00655-122">Relationships</span></span>
<span data-ttu-id="00655-123">Нет</span><span class="sxs-lookup"><span data-stu-id="00655-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00655-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00655-124">JSON Representation</span></span>
<span data-ttu-id="00655-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00655-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





