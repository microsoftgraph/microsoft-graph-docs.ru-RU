---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256674"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="af9cf-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="af9cf-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="af9cf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af9cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af9cf-105">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="af9cf-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="af9cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="af9cf-106">Properties</span></span>
|<span data-ttu-id="af9cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="af9cf-107">Property</span></span>|<span data-ttu-id="af9cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="af9cf-108">Type</span></span>|<span data-ttu-id="af9cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af9cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af9cf-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="af9cf-110">deviceAccount</span></span>|[<span data-ttu-id="af9cf-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="af9cf-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="af9cf-112">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af9cf-112">Not yet documented</span></span>|
|<span data-ttu-id="af9cf-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="af9cf-113">passwordRotationEnabled</span></span>|<span data-ttu-id="af9cf-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="af9cf-114">Boolean</span></span>|<span data-ttu-id="af9cf-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af9cf-115">Not yet documented</span></span>|
|<span data-ttu-id="af9cf-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="af9cf-116">calendarSyncEnabled</span></span>|<span data-ttu-id="af9cf-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="af9cf-117">Boolean</span></span>|<span data-ttu-id="af9cf-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af9cf-118">Not yet documented</span></span>|
|<span data-ttu-id="af9cf-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="af9cf-119">deviceAccountEmail</span></span>|<span data-ttu-id="af9cf-120">String</span><span class="sxs-lookup"><span data-stu-id="af9cf-120">String</span></span>|<span data-ttu-id="af9cf-121">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af9cf-121">Not yet documented</span></span>|
|<span data-ttu-id="af9cf-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="af9cf-122">exchangeServer</span></span>|<span data-ttu-id="af9cf-123">String</span><span class="sxs-lookup"><span data-stu-id="af9cf-123">String</span></span>|<span data-ttu-id="af9cf-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af9cf-124">Not yet documented</span></span>|
|<span data-ttu-id="af9cf-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="af9cf-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="af9cf-126">String</span><span class="sxs-lookup"><span data-stu-id="af9cf-126">String</span></span>|<span data-ttu-id="af9cf-127">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af9cf-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="af9cf-128">Связи</span><span class="sxs-lookup"><span data-stu-id="af9cf-128">Relationships</span></span>
<span data-ttu-id="af9cf-129">Нет</span><span class="sxs-lookup"><span data-stu-id="af9cf-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af9cf-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af9cf-130">JSON Representation</span></span>
<span data-ttu-id="af9cf-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af9cf-131">Here is a JSON representation of the resource.</span></span>
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



