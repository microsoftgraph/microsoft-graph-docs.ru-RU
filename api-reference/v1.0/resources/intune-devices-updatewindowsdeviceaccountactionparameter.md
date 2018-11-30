---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Н/Д
ms.openlocfilehash: f6403e4c3b106b318b7d551796911f6bcc0253c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026817"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="4dfbe-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="4dfbe-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="4dfbe-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4dfbe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dfbe-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4dfbe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dfbe-106">Properties</span></span>
|<span data-ttu-id="4dfbe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dfbe-107">Property</span></span>|<span data-ttu-id="4dfbe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4dfbe-108">Type</span></span>|<span data-ttu-id="4dfbe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4dfbe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dfbe-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="4dfbe-110">deviceAccount</span></span>|[<span data-ttu-id="4dfbe-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="4dfbe-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="4dfbe-112">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-112">Not yet documented</span></span>|
|<span data-ttu-id="4dfbe-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="4dfbe-113">passwordRotationEnabled</span></span>|<span data-ttu-id="4dfbe-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dfbe-114">Boolean</span></span>|<span data-ttu-id="4dfbe-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-115">Not yet documented</span></span>|
|<span data-ttu-id="4dfbe-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="4dfbe-116">calendarSyncEnabled</span></span>|<span data-ttu-id="4dfbe-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dfbe-117">Boolean</span></span>|<span data-ttu-id="4dfbe-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-118">Not yet documented</span></span>|
|<span data-ttu-id="4dfbe-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="4dfbe-119">deviceAccountEmail</span></span>|<span data-ttu-id="4dfbe-120">String</span><span class="sxs-lookup"><span data-stu-id="4dfbe-120">String</span></span>|<span data-ttu-id="4dfbe-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-121">Not yet documented</span></span>|
|<span data-ttu-id="4dfbe-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="4dfbe-122">exchangeServer</span></span>|<span data-ttu-id="4dfbe-123">String</span><span class="sxs-lookup"><span data-stu-id="4dfbe-123">String</span></span>|<span data-ttu-id="4dfbe-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-124">Not yet documented</span></span>|
|<span data-ttu-id="4dfbe-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="4dfbe-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="4dfbe-126">String</span><span class="sxs-lookup"><span data-stu-id="4dfbe-126">String</span></span>|<span data-ttu-id="4dfbe-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4dfbe-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dfbe-128">Связи</span><span class="sxs-lookup"><span data-stu-id="4dfbe-128">Relationships</span></span>
<span data-ttu-id="4dfbe-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4dfbe-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4dfbe-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dfbe-130">JSON Representation</span></span>
<span data-ttu-id="4dfbe-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dfbe-131">Here is a JSON representation of the resource.</span></span>
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



