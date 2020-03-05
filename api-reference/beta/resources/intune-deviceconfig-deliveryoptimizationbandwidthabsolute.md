---
title: Тип ресурса Деливерйоптимизатионбандвидсабсолуте
description: Пределы пропускной способности в килобайтах в секунду.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 536ba80fbc1ae0cee8bbef9933d6366a05284c33
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526820"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="351b7-103">Тип ресурса Деливерйоптимизатионбандвидсабсолуте</span><span class="sxs-lookup"><span data-stu-id="351b7-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="351b7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="351b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="351b7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="351b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="351b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="351b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="351b7-107">Пределы пропускной способности в килобайтах в секунду.</span><span class="sxs-lookup"><span data-stu-id="351b7-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="351b7-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="351b7-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="351b7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="351b7-109">Properties</span></span>
|<span data-ttu-id="351b7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="351b7-110">Property</span></span>|<span data-ttu-id="351b7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="351b7-111">Type</span></span>|<span data-ttu-id="351b7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="351b7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="351b7-113">максимумдовнлоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="351b7-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="351b7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="351b7-114">Int64</span></span>|<span data-ttu-id="351b7-115">Указывает максимальную пропускную способность скачивания в килобайтах/с, которую устройство может использовать для всех параллельных операций загрузки с помощью оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="351b7-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="351b7-116">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="351b7-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="351b7-117">Значение 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загружаемых файлов.</span><span class="sxs-lookup"><span data-stu-id="351b7-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="351b7-118">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="351b7-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="351b7-119">максимумуплоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="351b7-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="351b7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="351b7-120">Int64</span></span>|<span data-ttu-id="351b7-121">Указывает максимальную пропускную способность передачи в килобайтах/с, которая будет использоваться устройством для всех параллельных операций отправки с помощью оптимизации доставки (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="351b7-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="351b7-122">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="351b7-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="351b7-123">Значение по умолчанию — 0, что позволяет использовать неограниченную пропускную способность (оптимизирована для минимального использования полосы пропускания при загрузке).</span><span class="sxs-lookup"><span data-stu-id="351b7-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="351b7-124">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="351b7-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="351b7-125">Связи</span><span class="sxs-lookup"><span data-stu-id="351b7-125">Relationships</span></span>
<span data-ttu-id="351b7-126">Нет</span><span class="sxs-lookup"><span data-stu-id="351b7-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="351b7-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="351b7-127">JSON Representation</span></span>
<span data-ttu-id="351b7-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="351b7-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```



