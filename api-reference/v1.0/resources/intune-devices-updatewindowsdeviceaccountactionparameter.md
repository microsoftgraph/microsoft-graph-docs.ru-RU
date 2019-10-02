---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33b4b9e62b1038eb3b9e97b01a3d7b38906b605c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356894"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="c1155-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c1155-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="c1155-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1155-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1155-105">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="c1155-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c1155-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1155-106">Properties</span></span>
|<span data-ttu-id="c1155-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1155-107">Property</span></span>|<span data-ttu-id="c1155-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c1155-108">Type</span></span>|<span data-ttu-id="c1155-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c1155-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1155-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="c1155-110">deviceAccount</span></span>|[<span data-ttu-id="c1155-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="c1155-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="c1155-112">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1155-112">Not yet documented</span></span>|
|<span data-ttu-id="c1155-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="c1155-113">passwordRotationEnabled</span></span>|<span data-ttu-id="c1155-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1155-114">Boolean</span></span>|<span data-ttu-id="c1155-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c1155-115">Not yet documented</span></span>|
|<span data-ttu-id="c1155-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="c1155-116">calendarSyncEnabled</span></span>|<span data-ttu-id="c1155-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1155-117">Boolean</span></span>|<span data-ttu-id="c1155-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c1155-118">Not yet documented</span></span>|
|<span data-ttu-id="c1155-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="c1155-119">deviceAccountEmail</span></span>|<span data-ttu-id="c1155-120">String</span><span class="sxs-lookup"><span data-stu-id="c1155-120">String</span></span>|<span data-ttu-id="c1155-121">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1155-121">Not yet documented</span></span>|
|<span data-ttu-id="c1155-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="c1155-122">exchangeServer</span></span>|<span data-ttu-id="c1155-123">String</span><span class="sxs-lookup"><span data-stu-id="c1155-123">String</span></span>|<span data-ttu-id="c1155-124">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1155-124">Not yet documented</span></span>|
|<span data-ttu-id="c1155-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="c1155-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="c1155-126">String</span><span class="sxs-lookup"><span data-stu-id="c1155-126">String</span></span>|<span data-ttu-id="c1155-127">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1155-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1155-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c1155-128">Relationships</span></span>
<span data-ttu-id="c1155-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c1155-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1155-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1155-130">JSON Representation</span></span>
<span data-ttu-id="c1155-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1155-131">Here is a JSON representation of the resource.</span></span>
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




