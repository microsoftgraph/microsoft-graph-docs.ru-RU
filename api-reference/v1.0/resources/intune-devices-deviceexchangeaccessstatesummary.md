---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 170717617679a1a2dc05dc0e0f4f617fab78467d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530309"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="c6504-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c6504-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="c6504-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6504-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6504-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6504-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6504-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="c6504-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="c6504-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6504-107">Properties</span></span>
|<span data-ttu-id="c6504-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6504-108">Property</span></span>|<span data-ttu-id="c6504-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c6504-109">Type</span></span>|<span data-ttu-id="c6504-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c6504-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6504-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6504-111">allowedDeviceCount</span></span>|<span data-ttu-id="c6504-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c6504-112">Int32</span></span>|<span data-ttu-id="c6504-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="c6504-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="c6504-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6504-114">blockedDeviceCount</span></span>|<span data-ttu-id="c6504-115">Int32</span><span class="sxs-lookup"><span data-stu-id="c6504-115">Int32</span></span>|<span data-ttu-id="c6504-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="c6504-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="c6504-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6504-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="c6504-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c6504-118">Int32</span></span>|<span data-ttu-id="c6504-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="c6504-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="c6504-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6504-120">unknownDeviceCount</span></span>|<span data-ttu-id="c6504-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c6504-121">Int32</span></span>|<span data-ttu-id="c6504-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="c6504-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="c6504-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6504-123">unavailableDeviceCount</span></span>|<span data-ttu-id="c6504-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c6504-124">Int32</span></span>|<span data-ttu-id="c6504-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6504-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6504-126">Связи</span><span class="sxs-lookup"><span data-stu-id="c6504-126">Relationships</span></span>
<span data-ttu-id="c6504-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c6504-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6504-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6504-128">JSON Representation</span></span>
<span data-ttu-id="c6504-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6504-129">Here is a JSON representation of the resource.</span></span>
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




