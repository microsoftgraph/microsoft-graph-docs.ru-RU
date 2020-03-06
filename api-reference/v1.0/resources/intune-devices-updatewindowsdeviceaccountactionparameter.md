---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d349128b6b2e415f3930dc3938c354f890073629
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533241"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="ba361-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="ba361-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

<span data-ttu-id="ba361-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba361-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba361-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba361-106">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ba361-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ba361-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba361-107">Properties</span></span>
|<span data-ttu-id="ba361-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba361-108">Property</span></span>|<span data-ttu-id="ba361-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba361-109">Type</span></span>|<span data-ttu-id="ba361-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba361-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba361-111">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="ba361-111">deviceAccount</span></span>|[<span data-ttu-id="ba361-112">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="ba361-112">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="ba361-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba361-113">Not yet documented</span></span>|
|<span data-ttu-id="ba361-114">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="ba361-114">passwordRotationEnabled</span></span>|<span data-ttu-id="ba361-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba361-115">Boolean</span></span>|<span data-ttu-id="ba361-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba361-116">Not yet documented</span></span>|
|<span data-ttu-id="ba361-117">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="ba361-117">calendarSyncEnabled</span></span>|<span data-ttu-id="ba361-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba361-118">Boolean</span></span>|<span data-ttu-id="ba361-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba361-119">Not yet documented</span></span>|
|<span data-ttu-id="ba361-120">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ba361-120">deviceAccountEmail</span></span>|<span data-ttu-id="ba361-121">String</span><span class="sxs-lookup"><span data-stu-id="ba361-121">String</span></span>|<span data-ttu-id="ba361-122">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba361-122">Not yet documented</span></span>|
|<span data-ttu-id="ba361-123">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="ba361-123">exchangeServer</span></span>|<span data-ttu-id="ba361-124">String</span><span class="sxs-lookup"><span data-stu-id="ba361-124">String</span></span>|<span data-ttu-id="ba361-125">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba361-125">Not yet documented</span></span>|
|<span data-ttu-id="ba361-126">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="ba361-126">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="ba361-127">String</span><span class="sxs-lookup"><span data-stu-id="ba361-127">String</span></span>|<span data-ttu-id="ba361-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba361-128">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba361-129">Связи</span><span class="sxs-lookup"><span data-stu-id="ba361-129">Relationships</span></span>
<span data-ttu-id="ba361-130">Нет</span><span class="sxs-lookup"><span data-stu-id="ba361-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba361-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba361-131">JSON Representation</span></span>
<span data-ttu-id="ba361-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba361-132">Here is a JSON representation of the resource.</span></span>
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




