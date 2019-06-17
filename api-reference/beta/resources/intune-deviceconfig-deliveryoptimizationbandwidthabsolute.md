---
title: Тип ресурса Деливерйоптимизатионбандвидсабсолуте
description: Пределы пропускной способности в килобайтах в секунду.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 626c46c035ec4a7af44c06a31f7269cde96a2b8b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979720"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="961d2-103">Тип ресурса Деливерйоптимизатионбандвидсабсолуте</span><span class="sxs-lookup"><span data-stu-id="961d2-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="961d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="961d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="961d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="961d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="961d2-106">Пределы пропускной способности в килобайтах в секунду.</span><span class="sxs-lookup"><span data-stu-id="961d2-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="961d2-107">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="961d2-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="961d2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="961d2-108">Properties</span></span>
|<span data-ttu-id="961d2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="961d2-109">Property</span></span>|<span data-ttu-id="961d2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="961d2-110">Type</span></span>|<span data-ttu-id="961d2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="961d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="961d2-112">Максимумдовнлоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="961d2-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="961d2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="961d2-113">Int64</span></span>|<span data-ttu-id="961d2-114">Указывает максимальную пропускную способность скачивания в килобайтах/с, которую устройство может использовать для всех параллельных операций загрузки с помощью оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="961d2-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="961d2-115">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="961d2-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="961d2-116">Значение 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загружаемых файлов.</span><span class="sxs-lookup"><span data-stu-id="961d2-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="961d2-117">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="961d2-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="961d2-118">Максимумуплоадбандвидсинкилобитесперсеконд</span><span class="sxs-lookup"><span data-stu-id="961d2-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="961d2-119">Int64</span><span class="sxs-lookup"><span data-stu-id="961d2-119">Int64</span></span>|<span data-ttu-id="961d2-120">Указывает максимальную пропускную способность передачи в килобайтах/с, которая будет использоваться устройством для всех параллельных операций отправки с помощью оптимизации доставки (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="961d2-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="961d2-121">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="961d2-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="961d2-122">Значение по умолчанию — 0, что позволяет использовать неограниченную пропускную способность (оптимизирована для минимального использования полосы пропускания при загрузке).</span><span class="sxs-lookup"><span data-stu-id="961d2-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="961d2-123">Допустимые значения — от 0 до 4000000</span><span class="sxs-lookup"><span data-stu-id="961d2-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="961d2-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="961d2-124">Relationships</span></span>
<span data-ttu-id="961d2-125">Нет</span><span class="sxs-lookup"><span data-stu-id="961d2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="961d2-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="961d2-126">JSON Representation</span></span>
<span data-ttu-id="961d2-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="961d2-127">Here is a JSON representation of the resource.</span></span>
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





