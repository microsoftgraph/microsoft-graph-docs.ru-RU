---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76b3ca431bc68f93144a33dd8c5e8e5f036764a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140581"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="3733c-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="3733c-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="3733c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3733c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3733c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3733c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3733c-106">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="3733c-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="3733c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3733c-107">Properties</span></span>
|<span data-ttu-id="3733c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3733c-108">Property</span></span>|<span data-ttu-id="3733c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3733c-109">Type</span></span>|<span data-ttu-id="3733c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3733c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3733c-111">type</span><span class="sxs-lookup"><span data-stu-id="3733c-111">type</span></span>|[<span data-ttu-id="3733c-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="3733c-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="3733c-113">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="3733c-113">Device type.</span></span> <span data-ttu-id="3733c-114">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3733c-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="3733c-115">Минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="3733c-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="3733c-116">String</span><span class="sxs-lookup"><span data-stu-id="3733c-116">String</span></span>|<span data-ttu-id="3733c-117">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="3733c-117">Minimum OS version</span></span>|
|<span data-ttu-id="3733c-118">Максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="3733c-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="3733c-119">String</span><span class="sxs-lookup"><span data-stu-id="3733c-119">String</span></span>|<span data-ttu-id="3733c-120">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="3733c-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="3733c-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="3733c-121">Relationships</span></span>
<span data-ttu-id="3733c-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3733c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3733c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3733c-123">JSON Representation</span></span>
<span data-ttu-id="3733c-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3733c-124">Here is a JSON representation of the resource.</span></span>
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




