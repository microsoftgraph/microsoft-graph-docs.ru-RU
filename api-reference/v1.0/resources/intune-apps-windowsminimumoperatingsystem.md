---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
ms.openlocfilehash: ea1953bd0d58d4e578ffb7171fc157166072189b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314730"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="65244-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="65244-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="65244-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65244-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65244-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="65244-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="65244-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="65244-106">Properties</span></span>
|<span data-ttu-id="65244-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="65244-107">Property</span></span>|<span data-ttu-id="65244-108">Тип</span><span class="sxs-lookup"><span data-stu-id="65244-108">Type</span></span>|<span data-ttu-id="65244-109">Описание</span><span class="sxs-lookup"><span data-stu-id="65244-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65244-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="65244-110">v8_0</span></span>|<span data-ttu-id="65244-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="65244-111">Boolean</span></span>|<span data-ttu-id="65244-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="65244-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="65244-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="65244-113">v8_1</span></span>|<span data-ttu-id="65244-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="65244-114">Boolean</span></span>|<span data-ttu-id="65244-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="65244-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="65244-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="65244-116">v10_0</span></span>|<span data-ttu-id="65244-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="65244-117">Boolean</span></span>|<span data-ttu-id="65244-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="65244-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65244-119">Связи</span><span class="sxs-lookup"><span data-stu-id="65244-119">Relationships</span></span>
<span data-ttu-id="65244-120">Нет</span><span class="sxs-lookup"><span data-stu-id="65244-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65244-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65244-121">JSON Representation</span></span>
<span data-ttu-id="65244-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65244-122">Here is a JSON representation of the resource.</span></span>
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



