---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a01a1207801063285d7b59f0fa51c474ae78fb6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418556"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="12a1f-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="12a1f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="12a1f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12a1f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12a1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12a1f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12a1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a1f-107">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="12a1f-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="12a1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="12a1f-108">Properties</span></span>
|<span data-ttu-id="12a1f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="12a1f-109">Property</span></span>|<span data-ttu-id="12a1f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="12a1f-110">Type</span></span>|<span data-ttu-id="12a1f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12a1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a1f-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12a1f-112">allowedDeviceCount</span></span>|<span data-ttu-id="12a1f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="12a1f-113">Int32</span></span>|<span data-ttu-id="12a1f-114">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="12a1f-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="12a1f-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12a1f-115">blockedDeviceCount</span></span>|<span data-ttu-id="12a1f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="12a1f-116">Int32</span></span>|<span data-ttu-id="12a1f-117">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="12a1f-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="12a1f-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12a1f-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="12a1f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="12a1f-119">Int32</span></span>|<span data-ttu-id="12a1f-120">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="12a1f-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="12a1f-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12a1f-121">unknownDeviceCount</span></span>|<span data-ttu-id="12a1f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="12a1f-122">Int32</span></span>|<span data-ttu-id="12a1f-123">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="12a1f-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="12a1f-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12a1f-124">unavailableDeviceCount</span></span>|<span data-ttu-id="12a1f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="12a1f-125">Int32</span></span>|<span data-ttu-id="12a1f-126">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="12a1f-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12a1f-127">Связи</span><span class="sxs-lookup"><span data-stu-id="12a1f-127">Relationships</span></span>
<span data-ttu-id="12a1f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="12a1f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12a1f-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12a1f-129">JSON Representation</span></span>
<span data-ttu-id="12a1f-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12a1f-130">Here is a JSON representation of the resource.</span></span>
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




