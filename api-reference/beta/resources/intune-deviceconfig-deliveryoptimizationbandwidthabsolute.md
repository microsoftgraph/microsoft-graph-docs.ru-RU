---
title: Тип ресурса Деливерйоптимизатионбандвидсабсолуте
description: Пределы пропускной способности в килобайтах в секунду.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 710553bb01eb335eed9cf4075af3d87985239f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696253"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="ebe9c-103">Тип ресурса Деливерйоптимизатионбандвидсабсолуте</span><span class="sxs-lookup"><span data-stu-id="ebe9c-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="ebe9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebe9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebe9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebe9c-107">Пределы пропускной способности в килобайтах в секунду.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="ebe9c-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="ebe9c-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebe9c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebe9c-109">Properties</span></span>
|<span data-ttu-id="ebe9c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebe9c-110">Property</span></span>|<span data-ttu-id="ebe9c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ebe9c-111">Type</span></span>|<span data-ttu-id="ebe9c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ebe9c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe9c-113">максимумдовнлоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="ebe9c-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="ebe9c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ebe9c-114">Int64</span></span>|<span data-ttu-id="ebe9c-115">Указывает максимальную пропускную способность скачивания в килобайтах/с, которую устройство может использовать для всех параллельных операций загрузки с помощью оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="ebe9c-116">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="ebe9c-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="ebe9c-117">Значение 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загружаемых файлов.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="ebe9c-118">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="ebe9c-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="ebe9c-119">максимумуплоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="ebe9c-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="ebe9c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ebe9c-120">Int64</span></span>|<span data-ttu-id="ebe9c-121">Указывает максимальную пропускную способность передачи в килобайтах/с, которая будет использоваться устройством для всех параллельных операций отправки с помощью оптимизации доставки (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="ebe9c-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="ebe9c-122">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="ebe9c-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="ebe9c-123">Значение по умолчанию — 0, что позволяет использовать неограниченную пропускную способность (оптимизирована для минимального использования полосы пропускания при загрузке).</span><span class="sxs-lookup"><span data-stu-id="ebe9c-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="ebe9c-124">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="ebe9c-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebe9c-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ebe9c-125">Relationships</span></span>
<span data-ttu-id="ebe9c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ebe9c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebe9c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebe9c-127">JSON Representation</span></span>
<span data-ttu-id="ebe9c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebe9c-128">Here is a JSON representation of the resource.</span></span>
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





