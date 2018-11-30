---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
ms.openlocfilehash: 1b39890faf574ab952635c11f113c90479c3ba1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025259"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="726e5-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="726e5-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="726e5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="726e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="726e5-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="726e5-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="726e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="726e5-106">Properties</span></span>
|<span data-ttu-id="726e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="726e5-107">Property</span></span>|<span data-ttu-id="726e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="726e5-108">Type</span></span>|<span data-ttu-id="726e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="726e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="726e5-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="726e5-110">v8_0</span></span>|<span data-ttu-id="726e5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="726e5-111">Boolean</span></span>|<span data-ttu-id="726e5-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="726e5-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="726e5-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="726e5-113">v9_0</span></span>|<span data-ttu-id="726e5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="726e5-114">Boolean</span></span>|<span data-ttu-id="726e5-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="726e5-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="726e5-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="726e5-116">v10_0</span></span>|<span data-ttu-id="726e5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="726e5-117">Boolean</span></span>|<span data-ttu-id="726e5-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="726e5-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="726e5-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="726e5-119">v11_0</span></span>|<span data-ttu-id="726e5-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="726e5-120">Boolean</span></span>|<span data-ttu-id="726e5-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="726e5-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="726e5-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="726e5-122">v12_0</span></span>|<span data-ttu-id="726e5-123">Логический</span><span class="sxs-lookup"><span data-stu-id="726e5-123">Boolean</span></span>|<span data-ttu-id="726e5-124">12.0 или более поздняя версия.</span><span class="sxs-lookup"><span data-stu-id="726e5-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="726e5-125">Связи</span><span class="sxs-lookup"><span data-stu-id="726e5-125">Relationships</span></span>
<span data-ttu-id="726e5-126">Нет</span><span class="sxs-lookup"><span data-stu-id="726e5-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="726e5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="726e5-127">JSON Representation</span></span>
<span data-ttu-id="726e5-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="726e5-128">Here is a JSON representation of the resource.</span></span>
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



