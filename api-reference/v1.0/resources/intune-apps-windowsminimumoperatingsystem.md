---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d80a7c957b4a03132b349ebd609e21481322021a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863793"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="29df9-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="29df9-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="29df9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29df9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29df9-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="29df9-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="29df9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="29df9-106">Properties</span></span>
|<span data-ttu-id="29df9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="29df9-107">Property</span></span>|<span data-ttu-id="29df9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="29df9-108">Type</span></span>|<span data-ttu-id="29df9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="29df9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29df9-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="29df9-110">v8_0</span></span>|<span data-ttu-id="29df9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="29df9-111">Boolean</span></span>|<span data-ttu-id="29df9-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="29df9-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="29df9-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="29df9-113">v8_1</span></span>|<span data-ttu-id="29df9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="29df9-114">Boolean</span></span>|<span data-ttu-id="29df9-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="29df9-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="29df9-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="29df9-116">v10_0</span></span>|<span data-ttu-id="29df9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="29df9-117">Boolean</span></span>|<span data-ttu-id="29df9-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="29df9-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29df9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="29df9-119">Relationships</span></span>
<span data-ttu-id="29df9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="29df9-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29df9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29df9-121">JSON Representation</span></span>
<span data-ttu-id="29df9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29df9-122">Here is a JSON representation of the resource.</span></span>
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



