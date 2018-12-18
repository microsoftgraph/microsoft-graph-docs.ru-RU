---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Н/Д
author: tfitzmac
ms.openlocfilehash: cd69ffa01473a40228d53ad2f68f793cadf838d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335464"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="d3089-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="d3089-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="d3089-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d3089-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3089-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d3089-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3089-106">Properties</span></span>
|<span data-ttu-id="d3089-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3089-107">Property</span></span>|<span data-ttu-id="d3089-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d3089-108">Type</span></span>|<span data-ttu-id="d3089-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3089-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3089-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="d3089-110">deviceAccount</span></span>|[<span data-ttu-id="d3089-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="d3089-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="d3089-112">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-112">Not yet documented</span></span>|
|<span data-ttu-id="d3089-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="d3089-113">passwordRotationEnabled</span></span>|<span data-ttu-id="d3089-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3089-114">Boolean</span></span>|<span data-ttu-id="d3089-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-115">Not yet documented</span></span>|
|<span data-ttu-id="d3089-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="d3089-116">calendarSyncEnabled</span></span>|<span data-ttu-id="d3089-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3089-117">Boolean</span></span>|<span data-ttu-id="d3089-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-118">Not yet documented</span></span>|
|<span data-ttu-id="d3089-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="d3089-119">deviceAccountEmail</span></span>|<span data-ttu-id="d3089-120">String</span><span class="sxs-lookup"><span data-stu-id="d3089-120">String</span></span>|<span data-ttu-id="d3089-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-121">Not yet documented</span></span>|
|<span data-ttu-id="d3089-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="d3089-122">exchangeServer</span></span>|<span data-ttu-id="d3089-123">String</span><span class="sxs-lookup"><span data-stu-id="d3089-123">String</span></span>|<span data-ttu-id="d3089-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-124">Not yet documented</span></span>|
|<span data-ttu-id="d3089-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="d3089-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="d3089-126">String</span><span class="sxs-lookup"><span data-stu-id="d3089-126">String</span></span>|<span data-ttu-id="d3089-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3089-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3089-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d3089-128">Relationships</span></span>
<span data-ttu-id="d3089-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d3089-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3089-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3089-130">JSON Representation</span></span>
<span data-ttu-id="d3089-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3089-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



