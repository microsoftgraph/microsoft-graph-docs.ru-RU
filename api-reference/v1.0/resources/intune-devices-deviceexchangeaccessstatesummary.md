---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25bc1fe1592b2aa1a1f0cde1b4bf45b6092a36d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407038"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ba917-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ba917-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="ba917-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba917-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba917-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba917-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="ba917-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ba917-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba917-107">Properties</span></span>
|<span data-ttu-id="ba917-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba917-108">Property</span></span>|<span data-ttu-id="ba917-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba917-109">Type</span></span>|<span data-ttu-id="ba917-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba917-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba917-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba917-111">allowedDeviceCount</span></span>|<span data-ttu-id="ba917-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ba917-112">Int32</span></span>|<span data-ttu-id="ba917-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="ba917-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ba917-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba917-114">blockedDeviceCount</span></span>|<span data-ttu-id="ba917-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ba917-115">Int32</span></span>|<span data-ttu-id="ba917-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="ba917-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ba917-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba917-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="ba917-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ba917-118">Int32</span></span>|<span data-ttu-id="ba917-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="ba917-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ba917-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba917-120">unknownDeviceCount</span></span>|<span data-ttu-id="ba917-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ba917-121">Int32</span></span>|<span data-ttu-id="ba917-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="ba917-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ba917-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba917-123">unavailableDeviceCount</span></span>|<span data-ttu-id="ba917-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ba917-124">Int32</span></span>|<span data-ttu-id="ba917-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba917-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba917-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ba917-126">Relationships</span></span>
<span data-ttu-id="ba917-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ba917-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba917-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba917-128">JSON Representation</span></span>
<span data-ttu-id="ba917-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba917-129">Here is a JSON representation of the resource.</span></span>
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







