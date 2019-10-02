---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3210643c68a7b5a94bfa3b4f601a2e34efe68e13
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356978"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ef1fb-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ef1fb-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="ef1fb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef1fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef1fb-105">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="ef1fb-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ef1fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef1fb-106">Properties</span></span>
|<span data-ttu-id="ef1fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef1fb-107">Property</span></span>|<span data-ttu-id="ef1fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ef1fb-108">Type</span></span>|<span data-ttu-id="ef1fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ef1fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef1fb-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ef1fb-110">allowedDeviceCount</span></span>|<span data-ttu-id="ef1fb-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1fb-111">Int32</span></span>|<span data-ttu-id="ef1fb-112">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="ef1fb-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ef1fb-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ef1fb-113">blockedDeviceCount</span></span>|<span data-ttu-id="ef1fb-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1fb-114">Int32</span></span>|<span data-ttu-id="ef1fb-115">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="ef1fb-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ef1fb-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ef1fb-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="ef1fb-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1fb-117">Int32</span></span>|<span data-ttu-id="ef1fb-118">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="ef1fb-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ef1fb-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ef1fb-119">unknownDeviceCount</span></span>|<span data-ttu-id="ef1fb-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1fb-120">Int32</span></span>|<span data-ttu-id="ef1fb-121">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="ef1fb-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ef1fb-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ef1fb-122">unavailableDeviceCount</span></span>|<span data-ttu-id="ef1fb-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1fb-123">Int32</span></span>|<span data-ttu-id="ef1fb-124">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef1fb-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef1fb-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ef1fb-125">Relationships</span></span>
<span data-ttu-id="ef1fb-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ef1fb-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef1fb-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef1fb-127">JSON Representation</span></span>
<span data-ttu-id="ef1fb-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef1fb-128">Here is a JSON representation of the resource.</span></span>
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




