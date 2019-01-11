---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 10eb3738e14e8239f92f8578d01b9d4888b06b24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829822"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="48bd3-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="48bd3-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="48bd3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48bd3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48bd3-105">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="48bd3-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="48bd3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="48bd3-106">Properties</span></span>
|<span data-ttu-id="48bd3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="48bd3-107">Property</span></span>|<span data-ttu-id="48bd3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="48bd3-108">Type</span></span>|<span data-ttu-id="48bd3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="48bd3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48bd3-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48bd3-110">allowedDeviceCount</span></span>|<span data-ttu-id="48bd3-111">Int32</span><span class="sxs-lookup"><span data-stu-id="48bd3-111">Int32</span></span>|<span data-ttu-id="48bd3-112">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="48bd3-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="48bd3-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48bd3-113">blockedDeviceCount</span></span>|<span data-ttu-id="48bd3-114">Int32</span><span class="sxs-lookup"><span data-stu-id="48bd3-114">Int32</span></span>|<span data-ttu-id="48bd3-115">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="48bd3-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="48bd3-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48bd3-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="48bd3-117">Int32</span><span class="sxs-lookup"><span data-stu-id="48bd3-117">Int32</span></span>|<span data-ttu-id="48bd3-118">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="48bd3-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="48bd3-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48bd3-119">unknownDeviceCount</span></span>|<span data-ttu-id="48bd3-120">Int32</span><span class="sxs-lookup"><span data-stu-id="48bd3-120">Int32</span></span>|<span data-ttu-id="48bd3-121">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="48bd3-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="48bd3-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48bd3-122">unavailableDeviceCount</span></span>|<span data-ttu-id="48bd3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="48bd3-123">Int32</span></span>|<span data-ttu-id="48bd3-124">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="48bd3-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48bd3-125">Связи</span><span class="sxs-lookup"><span data-stu-id="48bd3-125">Relationships</span></span>
<span data-ttu-id="48bd3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="48bd3-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48bd3-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48bd3-127">JSON Representation</span></span>
<span data-ttu-id="48bd3-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48bd3-128">Here is a JSON representation of the resource.</span></span>
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



