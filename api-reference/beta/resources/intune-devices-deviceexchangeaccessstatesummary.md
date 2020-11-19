---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3221c3eaa8a02bf5fcbcd03385864e7d31aacb07
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293166"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="120a0-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="120a0-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="120a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="120a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="120a0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="120a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="120a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="120a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120a0-107">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="120a0-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="120a0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="120a0-108">Properties</span></span>
|<span data-ttu-id="120a0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="120a0-109">Property</span></span>|<span data-ttu-id="120a0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="120a0-110">Type</span></span>|<span data-ttu-id="120a0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="120a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120a0-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120a0-112">allowedDeviceCount</span></span>|<span data-ttu-id="120a0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="120a0-113">Int32</span></span>|<span data-ttu-id="120a0-114">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="120a0-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="120a0-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120a0-115">blockedDeviceCount</span></span>|<span data-ttu-id="120a0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="120a0-116">Int32</span></span>|<span data-ttu-id="120a0-117">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="120a0-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="120a0-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120a0-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="120a0-119">Int32</span><span class="sxs-lookup"><span data-stu-id="120a0-119">Int32</span></span>|<span data-ttu-id="120a0-120">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="120a0-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="120a0-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120a0-121">unknownDeviceCount</span></span>|<span data-ttu-id="120a0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="120a0-122">Int32</span></span>|<span data-ttu-id="120a0-123">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="120a0-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="120a0-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120a0-124">unavailableDeviceCount</span></span>|<span data-ttu-id="120a0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="120a0-125">Int32</span></span>|<span data-ttu-id="120a0-126">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="120a0-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="120a0-127">Связи</span><span class="sxs-lookup"><span data-stu-id="120a0-127">Relationships</span></span>
<span data-ttu-id="120a0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="120a0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="120a0-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="120a0-129">JSON Representation</span></span>
<span data-ttu-id="120a0-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="120a0-130">Here is a JSON representation of the resource.</span></span>
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




