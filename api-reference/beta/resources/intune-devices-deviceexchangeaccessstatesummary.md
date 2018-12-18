---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
ms.openlocfilehash: cb04de02e44f16534e9a57383e48d989a16f8582
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326602"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="da378-103">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="da378-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="da378-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da378-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da378-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da378-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da378-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="da378-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da378-107">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="da378-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="da378-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da378-108">Properties</span></span>
|<span data-ttu-id="da378-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da378-109">Property</span></span>|<span data-ttu-id="da378-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da378-110">Type</span></span>|<span data-ttu-id="da378-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da378-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da378-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="da378-112">allowedDeviceCount</span></span>|<span data-ttu-id="da378-113">Int32</span><span class="sxs-lookup"><span data-stu-id="da378-113">Int32</span></span>|<span data-ttu-id="da378-114">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="da378-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="da378-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="da378-115">blockedDeviceCount</span></span>|<span data-ttu-id="da378-116">Int32</span><span class="sxs-lookup"><span data-stu-id="da378-116">Int32</span></span>|<span data-ttu-id="da378-117">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="da378-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="da378-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="da378-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="da378-119">Int32</span><span class="sxs-lookup"><span data-stu-id="da378-119">Int32</span></span>|<span data-ttu-id="da378-120">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="da378-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="da378-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="da378-121">unknownDeviceCount</span></span>|<span data-ttu-id="da378-122">Int32</span><span class="sxs-lookup"><span data-stu-id="da378-122">Int32</span></span>|<span data-ttu-id="da378-123">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="da378-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="da378-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="da378-124">unavailableDeviceCount</span></span>|<span data-ttu-id="da378-125">Int32</span><span class="sxs-lookup"><span data-stu-id="da378-125">Int32</span></span>|<span data-ttu-id="da378-126">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="da378-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da378-127">Связи</span><span class="sxs-lookup"><span data-stu-id="da378-127">Relationships</span></span>
<span data-ttu-id="da378-128">Нет</span><span class="sxs-lookup"><span data-stu-id="da378-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da378-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da378-129">JSON Representation</span></span>
<span data-ttu-id="da378-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da378-130">Here is a JSON representation of the resource.</span></span>
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





