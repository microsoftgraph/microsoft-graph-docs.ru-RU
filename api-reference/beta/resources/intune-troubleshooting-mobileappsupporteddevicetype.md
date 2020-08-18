---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef5d013492125b16b14f2fe2c3613549df3b537e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791703"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="ff2e5-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="ff2e5-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="ff2e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff2e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff2e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff2e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2e5-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="ff2e5-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="ff2e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff2e5-108">Properties</span></span>
|<span data-ttu-id="ff2e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff2e5-109">Property</span></span>|<span data-ttu-id="ff2e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2e5-110">Type</span></span>|<span data-ttu-id="ff2e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2e5-112">type</span><span class="sxs-lookup"><span data-stu-id="ff2e5-112">type</span></span>|[<span data-ttu-id="ff2e5-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="ff2e5-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ff2e5-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="ff2e5-114">Device type.</span></span> <span data-ttu-id="ff2e5-115">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="ff2e5-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ff2e5-116">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="ff2e5-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="ff2e5-117">String</span><span class="sxs-lookup"><span data-stu-id="ff2e5-117">String</span></span>|<span data-ttu-id="ff2e5-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="ff2e5-118">Minimum OS version</span></span>|
|<span data-ttu-id="ff2e5-119">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="ff2e5-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="ff2e5-120">String</span><span class="sxs-lookup"><span data-stu-id="ff2e5-120">String</span></span>|<span data-ttu-id="ff2e5-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="ff2e5-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2e5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="ff2e5-122">Relationships</span></span>
<span data-ttu-id="ff2e5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ff2e5-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff2e5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff2e5-124">JSON Representation</span></span>
<span data-ttu-id="ff2e5-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff2e5-125">Here is a JSON representation of the resource.</span></span>
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



