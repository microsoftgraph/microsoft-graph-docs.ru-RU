---
title: тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a3e2fc78712997eebd31a874363f000b4ad761e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863571"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="6a272-103">тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="6a272-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="6a272-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a272-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a272-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a272-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a272-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a272-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="6a272-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="6a272-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a272-108">Properties</span></span>
|<span data-ttu-id="6a272-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a272-109">Property</span></span>|<span data-ttu-id="6a272-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a272-110">Type</span></span>|<span data-ttu-id="6a272-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a272-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a272-112">type</span><span class="sxs-lookup"><span data-stu-id="6a272-112">type</span></span>|[<span data-ttu-id="6a272-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="6a272-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6a272-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="6a272-114">Device type.</span></span> <span data-ttu-id="6a272-115">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` . `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="6a272-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="6a272-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6a272-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="6a272-117">String</span><span class="sxs-lookup"><span data-stu-id="6a272-117">String</span></span>|<span data-ttu-id="6a272-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="6a272-118">Minimum OS version</span></span>|
|<span data-ttu-id="6a272-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6a272-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="6a272-120">String</span><span class="sxs-lookup"><span data-stu-id="6a272-120">String</span></span>|<span data-ttu-id="6a272-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="6a272-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a272-122">Связи</span><span class="sxs-lookup"><span data-stu-id="6a272-122">Relationships</span></span>
<span data-ttu-id="6a272-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6a272-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a272-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a272-124">JSON Representation</span></span>
<span data-ttu-id="6a272-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a272-125">Here is a JSON representation of the resource.</span></span>
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




