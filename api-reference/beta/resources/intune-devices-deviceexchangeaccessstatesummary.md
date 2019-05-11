---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15b7a3e1f07694f0a75bb84bdad7640981639079
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942124"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="0287f-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="0287f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="0287f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0287f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0287f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0287f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0287f-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="0287f-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="0287f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0287f-107">Properties</span></span>
|<span data-ttu-id="0287f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0287f-108">Property</span></span>|<span data-ttu-id="0287f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0287f-109">Type</span></span>|<span data-ttu-id="0287f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0287f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0287f-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0287f-111">allowedDeviceCount</span></span>|<span data-ttu-id="0287f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0287f-112">Int32</span></span>|<span data-ttu-id="0287f-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="0287f-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="0287f-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0287f-114">blockedDeviceCount</span></span>|<span data-ttu-id="0287f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0287f-115">Int32</span></span>|<span data-ttu-id="0287f-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="0287f-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="0287f-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0287f-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="0287f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="0287f-118">Int32</span></span>|<span data-ttu-id="0287f-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="0287f-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="0287f-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0287f-120">unknownDeviceCount</span></span>|<span data-ttu-id="0287f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0287f-121">Int32</span></span>|<span data-ttu-id="0287f-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="0287f-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="0287f-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0287f-123">unavailableDeviceCount</span></span>|<span data-ttu-id="0287f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0287f-124">Int32</span></span>|<span data-ttu-id="0287f-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="0287f-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0287f-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0287f-126">Relationships</span></span>
<span data-ttu-id="0287f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0287f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0287f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0287f-128">JSON Representation</span></span>
<span data-ttu-id="0287f-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0287f-129">Here is a JSON representation of the resource.</span></span>
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




