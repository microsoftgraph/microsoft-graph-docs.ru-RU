---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb00b67fefecc4ef78e19e2c6e053b274e4145d4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266076"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="10375-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="10375-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="10375-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10375-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10375-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10375-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10375-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10375-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10375-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="10375-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="10375-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="10375-108">Properties</span></span>
|<span data-ttu-id="10375-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="10375-109">Property</span></span>|<span data-ttu-id="10375-110">Тип</span><span class="sxs-lookup"><span data-stu-id="10375-110">Type</span></span>|<span data-ttu-id="10375-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10375-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10375-112">type</span><span class="sxs-lookup"><span data-stu-id="10375-112">type</span></span>|[<span data-ttu-id="10375-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="10375-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="10375-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="10375-114">Device type.</span></span> <span data-ttu-id="10375-115">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="10375-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="10375-116">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="10375-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="10375-117">String</span><span class="sxs-lookup"><span data-stu-id="10375-117">String</span></span>|<span data-ttu-id="10375-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="10375-118">Minimum OS version</span></span>|
|<span data-ttu-id="10375-119">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="10375-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="10375-120">String</span><span class="sxs-lookup"><span data-stu-id="10375-120">String</span></span>|<span data-ttu-id="10375-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="10375-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="10375-122">Связи</span><span class="sxs-lookup"><span data-stu-id="10375-122">Relationships</span></span>
<span data-ttu-id="10375-123">Нет</span><span class="sxs-lookup"><span data-stu-id="10375-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10375-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10375-124">JSON Representation</span></span>
<span data-ttu-id="10375-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10375-125">Here is a JSON representation of the resource.</span></span>
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




