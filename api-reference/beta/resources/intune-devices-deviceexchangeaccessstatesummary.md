---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7f26e49217ea43e64e43e9cdd4cce4b88bae561
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785009"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="51b61-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="51b61-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="51b61-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51b61-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51b61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51b61-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="51b61-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="51b61-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51b61-107">Properties</span></span>
|<span data-ttu-id="51b61-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51b61-108">Property</span></span>|<span data-ttu-id="51b61-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51b61-109">Type</span></span>|<span data-ttu-id="51b61-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51b61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b61-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51b61-111">allowedDeviceCount</span></span>|<span data-ttu-id="51b61-112">Int32</span><span class="sxs-lookup"><span data-stu-id="51b61-112">Int32</span></span>|<span data-ttu-id="51b61-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="51b61-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="51b61-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51b61-114">blockedDeviceCount</span></span>|<span data-ttu-id="51b61-115">Int32</span><span class="sxs-lookup"><span data-stu-id="51b61-115">Int32</span></span>|<span data-ttu-id="51b61-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="51b61-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="51b61-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51b61-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="51b61-118">Int32</span><span class="sxs-lookup"><span data-stu-id="51b61-118">Int32</span></span>|<span data-ttu-id="51b61-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="51b61-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="51b61-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51b61-120">unknownDeviceCount</span></span>|<span data-ttu-id="51b61-121">Int32</span><span class="sxs-lookup"><span data-stu-id="51b61-121">Int32</span></span>|<span data-ttu-id="51b61-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="51b61-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="51b61-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51b61-123">unavailableDeviceCount</span></span>|<span data-ttu-id="51b61-124">Int32</span><span class="sxs-lookup"><span data-stu-id="51b61-124">Int32</span></span>|<span data-ttu-id="51b61-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="51b61-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51b61-126">Связи</span><span class="sxs-lookup"><span data-stu-id="51b61-126">Relationships</span></span>
<span data-ttu-id="51b61-127">Нет</span><span class="sxs-lookup"><span data-stu-id="51b61-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51b61-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51b61-128">JSON Representation</span></span>
<span data-ttu-id="51b61-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51b61-129">Here is a JSON representation of the resource.</span></span>
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



