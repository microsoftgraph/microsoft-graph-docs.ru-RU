---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bf29cf514e9d2915957ffb18dc618425d326751
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000013"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="15e50-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="15e50-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="15e50-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15e50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15e50-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15e50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e50-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="15e50-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="15e50-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15e50-107">Properties</span></span>
|<span data-ttu-id="15e50-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15e50-108">Property</span></span>|<span data-ttu-id="15e50-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15e50-109">Type</span></span>|<span data-ttu-id="15e50-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15e50-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e50-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15e50-111">allowedDeviceCount</span></span>|<span data-ttu-id="15e50-112">Int32</span><span class="sxs-lookup"><span data-stu-id="15e50-112">Int32</span></span>|<span data-ttu-id="15e50-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="15e50-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="15e50-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15e50-114">blockedDeviceCount</span></span>|<span data-ttu-id="15e50-115">Int32</span><span class="sxs-lookup"><span data-stu-id="15e50-115">Int32</span></span>|<span data-ttu-id="15e50-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="15e50-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="15e50-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15e50-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="15e50-118">Int32</span><span class="sxs-lookup"><span data-stu-id="15e50-118">Int32</span></span>|<span data-ttu-id="15e50-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="15e50-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="15e50-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15e50-120">unknownDeviceCount</span></span>|<span data-ttu-id="15e50-121">Int32</span><span class="sxs-lookup"><span data-stu-id="15e50-121">Int32</span></span>|<span data-ttu-id="15e50-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="15e50-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="15e50-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15e50-123">unavailableDeviceCount</span></span>|<span data-ttu-id="15e50-124">Int32</span><span class="sxs-lookup"><span data-stu-id="15e50-124">Int32</span></span>|<span data-ttu-id="15e50-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="15e50-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15e50-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="15e50-126">Relationships</span></span>
<span data-ttu-id="15e50-127">Нет</span><span class="sxs-lookup"><span data-stu-id="15e50-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15e50-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15e50-128">JSON Representation</span></span>
<span data-ttu-id="15e50-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15e50-129">Here is a JSON representation of the resource.</span></span>
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





