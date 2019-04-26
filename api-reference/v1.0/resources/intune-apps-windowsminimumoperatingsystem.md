---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571711"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="72be6-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="72be6-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="72be6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72be6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72be6-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="72be6-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="72be6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="72be6-106">Properties</span></span>
|<span data-ttu-id="72be6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="72be6-107">Property</span></span>|<span data-ttu-id="72be6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="72be6-108">Type</span></span>|<span data-ttu-id="72be6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72be6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72be6-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="72be6-110">v8_0</span></span>|<span data-ttu-id="72be6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="72be6-111">Boolean</span></span>|<span data-ttu-id="72be6-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="72be6-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="72be6-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="72be6-113">v8_1</span></span>|<span data-ttu-id="72be6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="72be6-114">Boolean</span></span>|<span data-ttu-id="72be6-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="72be6-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="72be6-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="72be6-116">v10_0</span></span>|<span data-ttu-id="72be6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="72be6-117">Boolean</span></span>|<span data-ttu-id="72be6-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="72be6-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72be6-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="72be6-119">Relationships</span></span>
<span data-ttu-id="72be6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="72be6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72be6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72be6-121">JSON Representation</span></span>
<span data-ttu-id="72be6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72be6-122">Here is a JSON representation of the resource.</span></span>
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



