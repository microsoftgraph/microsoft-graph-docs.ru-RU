---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb64307c12dcaf7b4e4fd0443001db7c6190c6fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091259"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="8b0cb-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8b0cb-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="8b0cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b0cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b0cb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b0cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b0cb-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="8b0cb-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="8b0cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b0cb-107">Properties</span></span>
|<span data-ttu-id="8b0cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b0cb-108">Property</span></span>|<span data-ttu-id="8b0cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b0cb-109">Type</span></span>|<span data-ttu-id="8b0cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b0cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b0cb-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0cb-111">allowedDeviceCount</span></span>|<span data-ttu-id="8b0cb-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0cb-112">Int32</span></span>|<span data-ttu-id="8b0cb-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="8b0cb-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="8b0cb-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0cb-114">blockedDeviceCount</span></span>|<span data-ttu-id="8b0cb-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0cb-115">Int32</span></span>|<span data-ttu-id="8b0cb-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="8b0cb-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="8b0cb-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0cb-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="8b0cb-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0cb-118">Int32</span></span>|<span data-ttu-id="8b0cb-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="8b0cb-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="8b0cb-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0cb-120">unknownDeviceCount</span></span>|<span data-ttu-id="8b0cb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0cb-121">Int32</span></span>|<span data-ttu-id="8b0cb-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="8b0cb-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="8b0cb-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b0cb-123">unavailableDeviceCount</span></span>|<span data-ttu-id="8b0cb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8b0cb-124">Int32</span></span>|<span data-ttu-id="8b0cb-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b0cb-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b0cb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="8b0cb-126">Relationships</span></span>
<span data-ttu-id="8b0cb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="8b0cb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b0cb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b0cb-128">JSON Representation</span></span>
<span data-ttu-id="8b0cb-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b0cb-129">Here is a JSON representation of the resource.</span></span>
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









