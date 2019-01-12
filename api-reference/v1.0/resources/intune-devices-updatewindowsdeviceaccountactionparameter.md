---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f62dce1364fca28e85b728e0b7571906488ebbee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986679"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="c4166-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c4166-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="c4166-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4166-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4166-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c4166-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4166-106">Properties</span></span>
|<span data-ttu-id="c4166-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4166-107">Property</span></span>|<span data-ttu-id="c4166-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c4166-108">Type</span></span>|<span data-ttu-id="c4166-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c4166-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4166-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="c4166-110">deviceAccount</span></span>|[<span data-ttu-id="c4166-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="c4166-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="c4166-112">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-112">Not yet documented</span></span>|
|<span data-ttu-id="c4166-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="c4166-113">passwordRotationEnabled</span></span>|<span data-ttu-id="c4166-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4166-114">Boolean</span></span>|<span data-ttu-id="c4166-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-115">Not yet documented</span></span>|
|<span data-ttu-id="c4166-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="c4166-116">calendarSyncEnabled</span></span>|<span data-ttu-id="c4166-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4166-117">Boolean</span></span>|<span data-ttu-id="c4166-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-118">Not yet documented</span></span>|
|<span data-ttu-id="c4166-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="c4166-119">deviceAccountEmail</span></span>|<span data-ttu-id="c4166-120">String</span><span class="sxs-lookup"><span data-stu-id="c4166-120">String</span></span>|<span data-ttu-id="c4166-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-121">Not yet documented</span></span>|
|<span data-ttu-id="c4166-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="c4166-122">exchangeServer</span></span>|<span data-ttu-id="c4166-123">String</span><span class="sxs-lookup"><span data-stu-id="c4166-123">String</span></span>|<span data-ttu-id="c4166-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-124">Not yet documented</span></span>|
|<span data-ttu-id="c4166-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="c4166-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="c4166-126">String</span><span class="sxs-lookup"><span data-stu-id="c4166-126">String</span></span>|<span data-ttu-id="c4166-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4166-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4166-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c4166-128">Relationships</span></span>
<span data-ttu-id="c4166-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c4166-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4166-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4166-130">JSON Representation</span></span>
<span data-ttu-id="c4166-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4166-131">Here is a JSON representation of the resource.</span></span>
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



