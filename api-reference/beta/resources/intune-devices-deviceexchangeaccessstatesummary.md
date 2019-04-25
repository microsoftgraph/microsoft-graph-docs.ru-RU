---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39f944b7559abf72d144f5c1608ec4efec014530
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549120"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="eb5dc-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="eb5dc-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="eb5dc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb5dc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb5dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb5dc-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="eb5dc-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="eb5dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb5dc-107">Properties</span></span>
|<span data-ttu-id="eb5dc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb5dc-108">Property</span></span>|<span data-ttu-id="eb5dc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eb5dc-109">Type</span></span>|<span data-ttu-id="eb5dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb5dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb5dc-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5dc-111">allowedDeviceCount</span></span>|<span data-ttu-id="eb5dc-112">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5dc-112">Int32</span></span>|<span data-ttu-id="eb5dc-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="eb5dc-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="eb5dc-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5dc-114">blockedDeviceCount</span></span>|<span data-ttu-id="eb5dc-115">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5dc-115">Int32</span></span>|<span data-ttu-id="eb5dc-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="eb5dc-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="eb5dc-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5dc-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="eb5dc-118">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5dc-118">Int32</span></span>|<span data-ttu-id="eb5dc-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="eb5dc-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="eb5dc-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5dc-120">unknownDeviceCount</span></span>|<span data-ttu-id="eb5dc-121">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5dc-121">Int32</span></span>|<span data-ttu-id="eb5dc-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="eb5dc-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="eb5dc-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5dc-123">unavailableDeviceCount</span></span>|<span data-ttu-id="eb5dc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5dc-124">Int32</span></span>|<span data-ttu-id="eb5dc-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb5dc-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb5dc-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="eb5dc-126">Relationships</span></span>
<span data-ttu-id="eb5dc-127">Нет</span><span class="sxs-lookup"><span data-stu-id="eb5dc-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb5dc-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb5dc-128">JSON Representation</span></span>
<span data-ttu-id="eb5dc-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb5dc-129">Here is a JSON representation of the resource.</span></span>
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





