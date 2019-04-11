---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba2998e1312d24fe6f86420cea883e6039f813a4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771798"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="cd709-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="cd709-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="cd709-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd709-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd709-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd709-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd709-106">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="cd709-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="cd709-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd709-107">Properties</span></span>
|<span data-ttu-id="cd709-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd709-108">Property</span></span>|<span data-ttu-id="cd709-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd709-109">Type</span></span>|<span data-ttu-id="cd709-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd709-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd709-111">type</span><span class="sxs-lookup"><span data-stu-id="cd709-111">type</span></span>|[<span data-ttu-id="cd709-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="cd709-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="cd709-113">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="cd709-113">Device type.</span></span> <span data-ttu-id="cd709-114">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cd709-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="cd709-115">Минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="cd709-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="cd709-116">String</span><span class="sxs-lookup"><span data-stu-id="cd709-116">String</span></span>|<span data-ttu-id="cd709-117">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="cd709-117">Minimum OS version</span></span>|
|<span data-ttu-id="cd709-118">Максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="cd709-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="cd709-119">String</span><span class="sxs-lookup"><span data-stu-id="cd709-119">String</span></span>|<span data-ttu-id="cd709-120">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="cd709-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd709-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd709-121">Relationships</span></span>
<span data-ttu-id="cd709-122">Нет</span><span class="sxs-lookup"><span data-stu-id="cd709-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd709-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd709-123">JSON Representation</span></span>
<span data-ttu-id="cd709-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd709-124">Here is a JSON representation of the resource.</span></span>
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



