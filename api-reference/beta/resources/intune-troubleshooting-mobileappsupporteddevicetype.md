---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31edf2c846acc9e940cb6decf83b2b71df98d910
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155827"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="763c8-103">Тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="763c8-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="763c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="763c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="763c8-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="763c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="763c8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="763c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="763c8-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="763c8-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="763c8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="763c8-108">Properties</span></span>
|<span data-ttu-id="763c8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="763c8-109">Property</span></span>|<span data-ttu-id="763c8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="763c8-110">Type</span></span>|<span data-ttu-id="763c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="763c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="763c8-112">type</span><span class="sxs-lookup"><span data-stu-id="763c8-112">type</span></span>|[<span data-ttu-id="763c8-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="763c8-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="763c8-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="763c8-114">Device type.</span></span> <span data-ttu-id="763c8-115">Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` , `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `linux` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="763c8-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `linux`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="763c8-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="763c8-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="763c8-117">String</span><span class="sxs-lookup"><span data-stu-id="763c8-117">String</span></span>|<span data-ttu-id="763c8-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="763c8-118">Minimum OS version</span></span>|
|<span data-ttu-id="763c8-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="763c8-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="763c8-120">String</span><span class="sxs-lookup"><span data-stu-id="763c8-120">String</span></span>|<span data-ttu-id="763c8-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="763c8-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="763c8-122">Связи</span><span class="sxs-lookup"><span data-stu-id="763c8-122">Relationships</span></span>
<span data-ttu-id="763c8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="763c8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="763c8-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="763c8-124">JSON Representation</span></span>
<span data-ttu-id="763c8-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="763c8-125">Here is a JSON representation of the resource.</span></span>
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




