---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49afbb3383035711bc950a9a7226a354ae78f0e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920431"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="1f623-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="1f623-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="1f623-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f623-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f623-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f623-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f623-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f623-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f623-107">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="1f623-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="1f623-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f623-108">Properties</span></span>
|<span data-ttu-id="1f623-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f623-109">Property</span></span>|<span data-ttu-id="1f623-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1f623-110">Type</span></span>|<span data-ttu-id="1f623-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f623-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f623-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f623-112">allowedDeviceCount</span></span>|<span data-ttu-id="1f623-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1f623-113">Int32</span></span>|<span data-ttu-id="1f623-114">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="1f623-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="1f623-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f623-115">blockedDeviceCount</span></span>|<span data-ttu-id="1f623-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1f623-116">Int32</span></span>|<span data-ttu-id="1f623-117">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="1f623-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="1f623-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f623-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="1f623-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1f623-119">Int32</span></span>|<span data-ttu-id="1f623-120">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="1f623-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="1f623-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f623-121">unknownDeviceCount</span></span>|<span data-ttu-id="1f623-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1f623-122">Int32</span></span>|<span data-ttu-id="1f623-123">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="1f623-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="1f623-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1f623-124">unavailableDeviceCount</span></span>|<span data-ttu-id="1f623-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1f623-125">Int32</span></span>|<span data-ttu-id="1f623-126">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f623-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f623-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1f623-127">Relationships</span></span>
<span data-ttu-id="1f623-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1f623-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f623-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f623-129">JSON Representation</span></span>
<span data-ttu-id="1f623-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f623-130">Here is a JSON representation of the resource.</span></span>
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





