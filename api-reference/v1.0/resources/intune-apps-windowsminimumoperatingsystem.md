---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 521b82448d58a831f88bdf9d548612aee86bcba6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972952"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="40da6-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40da6-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="40da6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40da6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40da6-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="40da6-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="40da6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="40da6-106">Properties</span></span>
|<span data-ttu-id="40da6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="40da6-107">Property</span></span>|<span data-ttu-id="40da6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="40da6-108">Type</span></span>|<span data-ttu-id="40da6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40da6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40da6-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="40da6-110">v8_0</span></span>|<span data-ttu-id="40da6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="40da6-111">Boolean</span></span>|<span data-ttu-id="40da6-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="40da6-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="40da6-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="40da6-113">v8_1</span></span>|<span data-ttu-id="40da6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="40da6-114">Boolean</span></span>|<span data-ttu-id="40da6-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="40da6-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="40da6-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="40da6-116">v10_0</span></span>|<span data-ttu-id="40da6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="40da6-117">Boolean</span></span>|<span data-ttu-id="40da6-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="40da6-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40da6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="40da6-119">Relationships</span></span>
<span data-ttu-id="40da6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="40da6-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40da6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40da6-121">JSON Representation</span></span>
<span data-ttu-id="40da6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40da6-122">Here is a JSON representation of the resource.</span></span>
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



