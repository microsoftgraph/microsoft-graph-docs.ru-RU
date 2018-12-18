---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
ms.openlocfilehash: 5583006d4654f4244120fd9d6f55fe03307dc1fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306050"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="21045-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="21045-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="21045-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21045-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21045-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="21045-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="21045-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="21045-106">Properties</span></span>
|<span data-ttu-id="21045-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="21045-107">Property</span></span>|<span data-ttu-id="21045-108">Тип</span><span class="sxs-lookup"><span data-stu-id="21045-108">Type</span></span>|<span data-ttu-id="21045-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21045-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21045-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="21045-110">v8_0</span></span>|<span data-ttu-id="21045-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="21045-111">Boolean</span></span>|<span data-ttu-id="21045-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="21045-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="21045-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="21045-113">v9_0</span></span>|<span data-ttu-id="21045-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="21045-114">Boolean</span></span>|<span data-ttu-id="21045-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="21045-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="21045-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="21045-116">v10_0</span></span>|<span data-ttu-id="21045-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="21045-117">Boolean</span></span>|<span data-ttu-id="21045-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="21045-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="21045-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="21045-119">v11_0</span></span>|<span data-ttu-id="21045-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="21045-120">Boolean</span></span>|<span data-ttu-id="21045-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="21045-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="21045-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="21045-122">v12_0</span></span>|<span data-ttu-id="21045-123">Boolean.</span><span class="sxs-lookup"><span data-stu-id="21045-123">Boolean</span></span>|<span data-ttu-id="21045-124">12.0 или более поздняя версия.</span><span class="sxs-lookup"><span data-stu-id="21045-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21045-125">Связи</span><span class="sxs-lookup"><span data-stu-id="21045-125">Relationships</span></span>
<span data-ttu-id="21045-126">Нет</span><span class="sxs-lookup"><span data-stu-id="21045-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21045-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21045-127">JSON Representation</span></span>
<span data-ttu-id="21045-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21045-128">Here is a JSON representation of the resource.</span></span>
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



