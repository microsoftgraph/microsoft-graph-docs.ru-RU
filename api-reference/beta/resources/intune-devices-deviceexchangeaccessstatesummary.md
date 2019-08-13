---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91f0b831beee100b4c88b23f2a92f2cc0aebbfee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320793"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ae8b5-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ae8b5-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="ae8b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae8b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae8b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae8b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae8b5-106">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="ae8b5-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ae8b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae8b5-107">Properties</span></span>
|<span data-ttu-id="ae8b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8b5-108">Property</span></span>|<span data-ttu-id="ae8b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8b5-109">Type</span></span>|<span data-ttu-id="ae8b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae8b5-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae8b5-111">allowedDeviceCount</span></span>|<span data-ttu-id="ae8b5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ae8b5-112">Int32</span></span>|<span data-ttu-id="ae8b5-113">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="ae8b5-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ae8b5-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae8b5-114">blockedDeviceCount</span></span>|<span data-ttu-id="ae8b5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ae8b5-115">Int32</span></span>|<span data-ttu-id="ae8b5-116">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="ae8b5-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ae8b5-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae8b5-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="ae8b5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ae8b5-118">Int32</span></span>|<span data-ttu-id="ae8b5-119">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="ae8b5-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ae8b5-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae8b5-120">unknownDeviceCount</span></span>|<span data-ttu-id="ae8b5-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ae8b5-121">Int32</span></span>|<span data-ttu-id="ae8b5-122">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="ae8b5-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ae8b5-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae8b5-123">unavailableDeviceCount</span></span>|<span data-ttu-id="ae8b5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ae8b5-124">Int32</span></span>|<span data-ttu-id="ae8b5-125">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae8b5-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae8b5-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="ae8b5-126">Relationships</span></span>
<span data-ttu-id="ae8b5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ae8b5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae8b5-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae8b5-128">JSON Representation</span></span>
<span data-ttu-id="ae8b5-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8b5-129">Here is a JSON representation of the resource.</span></span>
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



