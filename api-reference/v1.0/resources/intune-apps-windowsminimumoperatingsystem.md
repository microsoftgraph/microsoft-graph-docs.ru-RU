---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254466"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="ba977-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba977-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="ba977-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba977-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba977-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="ba977-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="ba977-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba977-106">Properties</span></span>
|<span data-ttu-id="ba977-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba977-107">Property</span></span>|<span data-ttu-id="ba977-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ba977-108">Type</span></span>|<span data-ttu-id="ba977-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ba977-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba977-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="ba977-110">v8_0</span></span>|<span data-ttu-id="ba977-111">Логический</span><span class="sxs-lookup"><span data-stu-id="ba977-111">Boolean</span></span>|<span data-ttu-id="ba977-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="ba977-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="ba977-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="ba977-113">v8_1</span></span>|<span data-ttu-id="ba977-114">Логический</span><span class="sxs-lookup"><span data-stu-id="ba977-114">Boolean</span></span>|<span data-ttu-id="ba977-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="ba977-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="ba977-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="ba977-116">v10_0</span></span>|<span data-ttu-id="ba977-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba977-117">Boolean</span></span>|<span data-ttu-id="ba977-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="ba977-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba977-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ba977-119">Relationships</span></span>
<span data-ttu-id="ba977-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ba977-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba977-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba977-121">JSON Representation</span></span>
<span data-ttu-id="ba977-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba977-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



