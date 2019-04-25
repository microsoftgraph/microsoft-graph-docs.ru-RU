---
title: Тип ресурса updateWindowsDeviceAccountActionParameter
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523310"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="a01cb-103">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="a01cb-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="a01cb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a01cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a01cb-105">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="a01cb-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a01cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a01cb-106">Properties</span></span>
|<span data-ttu-id="a01cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a01cb-107">Property</span></span>|<span data-ttu-id="a01cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a01cb-108">Type</span></span>|<span data-ttu-id="a01cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a01cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a01cb-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="a01cb-110">deviceAccount</span></span>|[<span data-ttu-id="a01cb-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="a01cb-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="a01cb-112">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a01cb-112">Not yet documented</span></span>|
|<span data-ttu-id="a01cb-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="a01cb-113">passwordRotationEnabled</span></span>|<span data-ttu-id="a01cb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a01cb-114">Boolean</span></span>|<span data-ttu-id="a01cb-115">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a01cb-115">Not yet documented</span></span>|
|<span data-ttu-id="a01cb-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="a01cb-116">calendarSyncEnabled</span></span>|<span data-ttu-id="a01cb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a01cb-117">Boolean</span></span>|<span data-ttu-id="a01cb-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a01cb-118">Not yet documented</span></span>|
|<span data-ttu-id="a01cb-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="a01cb-119">deviceAccountEmail</span></span>|<span data-ttu-id="a01cb-120">String</span><span class="sxs-lookup"><span data-stu-id="a01cb-120">String</span></span>|<span data-ttu-id="a01cb-121">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a01cb-121">Not yet documented</span></span>|
|<span data-ttu-id="a01cb-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="a01cb-122">exchangeServer</span></span>|<span data-ttu-id="a01cb-123">String</span><span class="sxs-lookup"><span data-stu-id="a01cb-123">String</span></span>|<span data-ttu-id="a01cb-124">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a01cb-124">Not yet documented</span></span>|
|<span data-ttu-id="a01cb-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="a01cb-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="a01cb-126">String</span><span class="sxs-lookup"><span data-stu-id="a01cb-126">String</span></span>|<span data-ttu-id="a01cb-127">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a01cb-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a01cb-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="a01cb-128">Relationships</span></span>
<span data-ttu-id="a01cb-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a01cb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a01cb-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a01cb-130">JSON Representation</span></span>
<span data-ttu-id="a01cb-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a01cb-131">Here is a JSON representation of the resource.</span></span>
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



