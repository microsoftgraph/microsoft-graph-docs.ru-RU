---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b975dbe09a5c1b277b55bfb7f13405d9871bd1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030844"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="e5191-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="e5191-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="e5191-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5191-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5191-105">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="e5191-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="e5191-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5191-106">Properties</span></span>
|<span data-ttu-id="e5191-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5191-107">Property</span></span>|<span data-ttu-id="e5191-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e5191-108">Type</span></span>|<span data-ttu-id="e5191-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e5191-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5191-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5191-110">allowedDeviceCount</span></span>|<span data-ttu-id="e5191-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e5191-111">Int32</span></span>|<span data-ttu-id="e5191-112">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="e5191-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="e5191-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5191-113">blockedDeviceCount</span></span>|<span data-ttu-id="e5191-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e5191-114">Int32</span></span>|<span data-ttu-id="e5191-115">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="e5191-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="e5191-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5191-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="e5191-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e5191-117">Int32</span></span>|<span data-ttu-id="e5191-118">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="e5191-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="e5191-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5191-119">unknownDeviceCount</span></span>|<span data-ttu-id="e5191-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e5191-120">Int32</span></span>|<span data-ttu-id="e5191-121">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="e5191-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="e5191-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5191-122">unavailableDeviceCount</span></span>|<span data-ttu-id="e5191-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e5191-123">Int32</span></span>|<span data-ttu-id="e5191-124">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5191-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5191-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="e5191-125">Relationships</span></span>
<span data-ttu-id="e5191-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e5191-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5191-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5191-127">JSON Representation</span></span>
<span data-ttu-id="e5191-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5191-128">Here is a JSON representation of the resource.</span></span>
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



