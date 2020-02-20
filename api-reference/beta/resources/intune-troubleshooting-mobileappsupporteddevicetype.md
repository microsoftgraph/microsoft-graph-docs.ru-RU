---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b71c9ec708efb36f677e563992eca4130f347c80
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159075"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="d1784-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="d1784-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="d1784-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1784-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1784-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1784-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1784-106">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="d1784-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="d1784-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1784-107">Properties</span></span>
|<span data-ttu-id="d1784-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1784-108">Property</span></span>|<span data-ttu-id="d1784-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d1784-109">Type</span></span>|<span data-ttu-id="d1784-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1784-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1784-111">type</span><span class="sxs-lookup"><span data-stu-id="d1784-111">type</span></span>|[<span data-ttu-id="d1784-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="d1784-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d1784-113">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="d1784-113">Device type.</span></span> <span data-ttu-id="d1784-114">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="d1784-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d1784-115">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="d1784-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="d1784-116">String</span><span class="sxs-lookup"><span data-stu-id="d1784-116">String</span></span>|<span data-ttu-id="d1784-117">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="d1784-117">Minimum OS version</span></span>|
|<span data-ttu-id="d1784-118">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="d1784-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="d1784-119">String</span><span class="sxs-lookup"><span data-stu-id="d1784-119">String</span></span>|<span data-ttu-id="d1784-120">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="d1784-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1784-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1784-121">Relationships</span></span>
<span data-ttu-id="d1784-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d1784-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1784-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1784-123">JSON Representation</span></span>
<span data-ttu-id="d1784-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1784-124">Here is a JSON representation of the resource.</span></span>
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



