---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cee2a17eb6cacab64488693f3a6a6580f3fb3264
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317782"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="ae2d4-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="ae2d4-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="ae2d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae2d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae2d4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae2d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae2d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae2d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae2d4-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="ae2d4-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="ae2d4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae2d4-108">Properties</span></span>
|<span data-ttu-id="ae2d4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae2d4-109">Property</span></span>|<span data-ttu-id="ae2d4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ae2d4-110">Type</span></span>|<span data-ttu-id="ae2d4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ae2d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae2d4-112">type</span><span class="sxs-lookup"><span data-stu-id="ae2d4-112">type</span></span>|[<span data-ttu-id="ae2d4-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="ae2d4-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ae2d4-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="ae2d4-114">Device type.</span></span> <span data-ttu-id="ae2d4-115">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="ae2d4-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ae2d4-116">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="ae2d4-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="ae2d4-117">String</span><span class="sxs-lookup"><span data-stu-id="ae2d4-117">String</span></span>|<span data-ttu-id="ae2d4-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="ae2d4-118">Minimum OS version</span></span>|
|<span data-ttu-id="ae2d4-119">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="ae2d4-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="ae2d4-120">String</span><span class="sxs-lookup"><span data-stu-id="ae2d4-120">String</span></span>|<span data-ttu-id="ae2d4-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="ae2d4-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae2d4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="ae2d4-122">Relationships</span></span>
<span data-ttu-id="ae2d4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ae2d4-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae2d4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae2d4-124">JSON Representation</span></span>
<span data-ttu-id="ae2d4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae2d4-125">Here is a JSON representation of the resource.</span></span>
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



