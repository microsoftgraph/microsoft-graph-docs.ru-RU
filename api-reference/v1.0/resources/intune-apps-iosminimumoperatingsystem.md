---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254571"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="bda33-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bda33-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="bda33-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bda33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bda33-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="bda33-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="bda33-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bda33-106">Properties</span></span>
|<span data-ttu-id="bda33-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bda33-107">Property</span></span>|<span data-ttu-id="bda33-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bda33-108">Type</span></span>|<span data-ttu-id="bda33-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bda33-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda33-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="bda33-110">v8_0</span></span>|<span data-ttu-id="bda33-111">Логический</span><span class="sxs-lookup"><span data-stu-id="bda33-111">Boolean</span></span>|<span data-ttu-id="bda33-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="bda33-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="bda33-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="bda33-113">v9_0</span></span>|<span data-ttu-id="bda33-114">Логический</span><span class="sxs-lookup"><span data-stu-id="bda33-114">Boolean</span></span>|<span data-ttu-id="bda33-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="bda33-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="bda33-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="bda33-116">v10_0</span></span>|<span data-ttu-id="bda33-117">Логический</span><span class="sxs-lookup"><span data-stu-id="bda33-117">Boolean</span></span>|<span data-ttu-id="bda33-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="bda33-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="bda33-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="bda33-119">v11_0</span></span>|<span data-ttu-id="bda33-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="bda33-120">Boolean</span></span>|<span data-ttu-id="bda33-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="bda33-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="bda33-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="bda33-122">v12_0</span></span>|<span data-ttu-id="bda33-123">Логический</span><span class="sxs-lookup"><span data-stu-id="bda33-123">Boolean</span></span>|<span data-ttu-id="bda33-124">Версия 12,0 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="bda33-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda33-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="bda33-125">Relationships</span></span>
<span data-ttu-id="bda33-126">Нет</span><span class="sxs-lookup"><span data-stu-id="bda33-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bda33-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bda33-127">JSON Representation</span></span>
<span data-ttu-id="bda33-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bda33-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



