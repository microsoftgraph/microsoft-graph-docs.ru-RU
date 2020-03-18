---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: efd91d4ab3e4f267faf371cdb9ef3e828c59ffe1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764595"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="93e35-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="93e35-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="93e35-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93e35-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93e35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93e35-106">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="93e35-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="93e35-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="93e35-107">Properties</span></span>
|<span data-ttu-id="93e35-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="93e35-108">Property</span></span>|<span data-ttu-id="93e35-109">Тип</span><span class="sxs-lookup"><span data-stu-id="93e35-109">Type</span></span>|<span data-ttu-id="93e35-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93e35-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93e35-111">type</span><span class="sxs-lookup"><span data-stu-id="93e35-111">type</span></span>|[<span data-ttu-id="93e35-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="93e35-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="93e35-113">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="93e35-113">Device type.</span></span> <span data-ttu-id="93e35-114">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="93e35-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="93e35-115">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="93e35-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="93e35-116">String</span><span class="sxs-lookup"><span data-stu-id="93e35-116">String</span></span>|<span data-ttu-id="93e35-117">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="93e35-117">Minimum OS version</span></span>|
|<span data-ttu-id="93e35-118">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="93e35-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="93e35-119">String</span><span class="sxs-lookup"><span data-stu-id="93e35-119">String</span></span>|<span data-ttu-id="93e35-120">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="93e35-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="93e35-121">Связи</span><span class="sxs-lookup"><span data-stu-id="93e35-121">Relationships</span></span>
<span data-ttu-id="93e35-122">Нет</span><span class="sxs-lookup"><span data-stu-id="93e35-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93e35-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93e35-123">JSON Representation</span></span>
<span data-ttu-id="93e35-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e35-124">Here is a JSON representation of the resource.</span></span>
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



