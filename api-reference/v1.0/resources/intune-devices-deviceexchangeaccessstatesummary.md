---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260517"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="6d11a-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6d11a-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="6d11a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d11a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d11a-105">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="6d11a-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="6d11a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d11a-106">Properties</span></span>
|<span data-ttu-id="6d11a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d11a-107">Property</span></span>|<span data-ttu-id="6d11a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6d11a-108">Type</span></span>|<span data-ttu-id="6d11a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6d11a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d11a-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d11a-110">allowedDeviceCount</span></span>|<span data-ttu-id="6d11a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="6d11a-111">Int32</span></span>|<span data-ttu-id="6d11a-112">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="6d11a-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="6d11a-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d11a-113">blockedDeviceCount</span></span>|<span data-ttu-id="6d11a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6d11a-114">Int32</span></span>|<span data-ttu-id="6d11a-115">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="6d11a-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="6d11a-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d11a-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="6d11a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="6d11a-117">Int32</span></span>|<span data-ttu-id="6d11a-118">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="6d11a-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="6d11a-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d11a-119">unknownDeviceCount</span></span>|<span data-ttu-id="6d11a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6d11a-120">Int32</span></span>|<span data-ttu-id="6d11a-121">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="6d11a-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="6d11a-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d11a-122">unavailableDeviceCount</span></span>|<span data-ttu-id="6d11a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6d11a-123">Int32</span></span>|<span data-ttu-id="6d11a-124">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d11a-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d11a-125">Связи</span><span class="sxs-lookup"><span data-stu-id="6d11a-125">Relationships</span></span>
<span data-ttu-id="6d11a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6d11a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d11a-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d11a-127">JSON Representation</span></span>
<span data-ttu-id="6d11a-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d11a-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



