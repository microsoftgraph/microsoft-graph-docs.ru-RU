---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a80de09abe7e5fb513c95006f6b2c2fe719a4f39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925940"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="c221b-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c221b-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="c221b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c221b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c221b-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="c221b-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="c221b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c221b-106">Properties</span></span>
|<span data-ttu-id="c221b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c221b-107">Property</span></span>|<span data-ttu-id="c221b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c221b-108">Type</span></span>|<span data-ttu-id="c221b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c221b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c221b-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="c221b-110">v8_0</span></span>|<span data-ttu-id="c221b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="c221b-111">Boolean</span></span>|<span data-ttu-id="c221b-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c221b-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="c221b-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="c221b-113">v9_0</span></span>|<span data-ttu-id="c221b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c221b-114">Boolean</span></span>|<span data-ttu-id="c221b-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c221b-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="c221b-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="c221b-116">v10_0</span></span>|<span data-ttu-id="c221b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c221b-117">Boolean</span></span>|<span data-ttu-id="c221b-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c221b-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="c221b-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="c221b-119">v11_0</span></span>|<span data-ttu-id="c221b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c221b-120">Boolean</span></span>|<span data-ttu-id="c221b-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c221b-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="c221b-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="c221b-122">v12_0</span></span>|<span data-ttu-id="c221b-123">Логический</span><span class="sxs-lookup"><span data-stu-id="c221b-123">Boolean</span></span>|<span data-ttu-id="c221b-124">12.0 или более поздняя версия.</span><span class="sxs-lookup"><span data-stu-id="c221b-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c221b-125">Связи</span><span class="sxs-lookup"><span data-stu-id="c221b-125">Relationships</span></span>
<span data-ttu-id="c221b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c221b-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c221b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c221b-127">JSON Representation</span></span>
<span data-ttu-id="c221b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c221b-128">Here is a JSON representation of the resource.</span></span>
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



