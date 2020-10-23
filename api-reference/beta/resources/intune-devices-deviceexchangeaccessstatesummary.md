---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd20f76a810f37fde239cb523800d98bd8246700
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728239"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ee333-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ee333-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="ee333-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee333-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee333-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee333-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee333-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee333-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee333-107">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="ee333-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ee333-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee333-108">Properties</span></span>
|<span data-ttu-id="ee333-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee333-109">Property</span></span>|<span data-ttu-id="ee333-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ee333-110">Type</span></span>|<span data-ttu-id="ee333-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee333-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee333-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee333-112">allowedDeviceCount</span></span>|<span data-ttu-id="ee333-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ee333-113">Int32</span></span>|<span data-ttu-id="ee333-114">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="ee333-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ee333-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee333-115">blockedDeviceCount</span></span>|<span data-ttu-id="ee333-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ee333-116">Int32</span></span>|<span data-ttu-id="ee333-117">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="ee333-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ee333-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee333-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="ee333-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ee333-119">Int32</span></span>|<span data-ttu-id="ee333-120">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="ee333-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ee333-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee333-121">unknownDeviceCount</span></span>|<span data-ttu-id="ee333-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ee333-122">Int32</span></span>|<span data-ttu-id="ee333-123">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="ee333-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ee333-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee333-124">unavailableDeviceCount</span></span>|<span data-ttu-id="ee333-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ee333-125">Int32</span></span>|<span data-ttu-id="ee333-126">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee333-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee333-127">Связи</span><span class="sxs-lookup"><span data-stu-id="ee333-127">Relationships</span></span>
<span data-ttu-id="ee333-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ee333-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee333-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee333-129">JSON Representation</span></span>
<span data-ttu-id="ee333-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee333-130">Here is a JSON representation of the resource.</span></span>
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





