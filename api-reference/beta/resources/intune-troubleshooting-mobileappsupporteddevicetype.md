---
title: Тип ресурса Мобилеаппсуппортеддевицетипе
description: Свойства устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8e0b0f6232645dfff0e59e8d1ff808e47ff472
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523326"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="47d44-103">Тип ресурса Мобилеаппсуппортеддевицетипе</span><span class="sxs-lookup"><span data-stu-id="47d44-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="47d44-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47d44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d44-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d44-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47d44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d44-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="47d44-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="47d44-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47d44-108">Properties</span></span>
|<span data-ttu-id="47d44-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d44-109">Property</span></span>|<span data-ttu-id="47d44-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47d44-110">Type</span></span>|<span data-ttu-id="47d44-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47d44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d44-112">type</span><span class="sxs-lookup"><span data-stu-id="47d44-112">type</span></span>|[<span data-ttu-id="47d44-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="47d44-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="47d44-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="47d44-114">Device type.</span></span> <span data-ttu-id="47d44-115">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="47d44-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="47d44-116">минимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="47d44-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="47d44-117">String</span><span class="sxs-lookup"><span data-stu-id="47d44-117">String</span></span>|<span data-ttu-id="47d44-118">Минимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="47d44-118">Minimum OS version</span></span>|
|<span data-ttu-id="47d44-119">максимумоператингсистемверсион</span><span class="sxs-lookup"><span data-stu-id="47d44-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="47d44-120">String</span><span class="sxs-lookup"><span data-stu-id="47d44-120">String</span></span>|<span data-ttu-id="47d44-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="47d44-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="47d44-122">Связи</span><span class="sxs-lookup"><span data-stu-id="47d44-122">Relationships</span></span>
<span data-ttu-id="47d44-123">Нет</span><span class="sxs-lookup"><span data-stu-id="47d44-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47d44-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47d44-124">JSON Representation</span></span>
<span data-ttu-id="47d44-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47d44-125">Here is a JSON representation of the resource.</span></span>
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



