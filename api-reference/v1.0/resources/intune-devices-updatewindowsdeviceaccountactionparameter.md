---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 536f69a30e5da74bfbfe1785b71f642dc324a38f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867286"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="06364-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="06364-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="06364-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06364-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06364-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="06364-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="06364-106">Properties</span></span>
|<span data-ttu-id="06364-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="06364-107">Property</span></span>|<span data-ttu-id="06364-108">Тип</span><span class="sxs-lookup"><span data-stu-id="06364-108">Type</span></span>|<span data-ttu-id="06364-109">Описание</span><span class="sxs-lookup"><span data-stu-id="06364-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06364-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="06364-110">deviceAccount</span></span>|[<span data-ttu-id="06364-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="06364-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="06364-112">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-112">Not yet documented</span></span>|
|<span data-ttu-id="06364-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="06364-113">passwordRotationEnabled</span></span>|<span data-ttu-id="06364-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="06364-114">Boolean</span></span>|<span data-ttu-id="06364-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-115">Not yet documented</span></span>|
|<span data-ttu-id="06364-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="06364-116">calendarSyncEnabled</span></span>|<span data-ttu-id="06364-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="06364-117">Boolean</span></span>|<span data-ttu-id="06364-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-118">Not yet documented</span></span>|
|<span data-ttu-id="06364-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="06364-119">deviceAccountEmail</span></span>|<span data-ttu-id="06364-120">String</span><span class="sxs-lookup"><span data-stu-id="06364-120">String</span></span>|<span data-ttu-id="06364-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-121">Not yet documented</span></span>|
|<span data-ttu-id="06364-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="06364-122">exchangeServer</span></span>|<span data-ttu-id="06364-123">String</span><span class="sxs-lookup"><span data-stu-id="06364-123">String</span></span>|<span data-ttu-id="06364-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-124">Not yet documented</span></span>|
|<span data-ttu-id="06364-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="06364-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="06364-126">String</span><span class="sxs-lookup"><span data-stu-id="06364-126">String</span></span>|<span data-ttu-id="06364-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06364-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="06364-128">Связи</span><span class="sxs-lookup"><span data-stu-id="06364-128">Relationships</span></span>
<span data-ttu-id="06364-129">Нет</span><span class="sxs-lookup"><span data-stu-id="06364-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06364-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06364-130">JSON Representation</span></span>
<span data-ttu-id="06364-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06364-131">Here is a JSON representation of the resource.</span></span>
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



