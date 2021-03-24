---
title: тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 559dc38a5fc8d2e9b7142efb43d83a97f29db10c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141381"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="cdc6b-103">тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="cdc6b-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="cdc6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdc6b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdc6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc6b-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="cdc6b-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="cdc6b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdc6b-108">Properties</span></span>
|<span data-ttu-id="cdc6b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdc6b-109">Property</span></span>|<span data-ttu-id="cdc6b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cdc6b-110">Type</span></span>|<span data-ttu-id="cdc6b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc6b-112">type</span><span class="sxs-lookup"><span data-stu-id="cdc6b-112">type</span></span>|[<span data-ttu-id="cdc6b-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="cdc6b-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="cdc6b-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="cdc6b-114">Device type.</span></span> <span data-ttu-id="cdc6b-115">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` , `unknown` `cloudPC` , .</span><span class="sxs-lookup"><span data-stu-id="cdc6b-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="cdc6b-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cdc6b-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="cdc6b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="cdc6b-117">String</span></span>|<span data-ttu-id="cdc6b-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="cdc6b-118">Minimum OS version</span></span>|
|<span data-ttu-id="cdc6b-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cdc6b-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="cdc6b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="cdc6b-120">String</span></span>|<span data-ttu-id="cdc6b-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="cdc6b-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdc6b-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="cdc6b-122">Relationships</span></span>
<span data-ttu-id="cdc6b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cdc6b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdc6b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cdc6b-124">JSON Representation</span></span>
<span data-ttu-id="cdc6b-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdc6b-125">Here is a JSON representation of the resource.</span></span>
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




