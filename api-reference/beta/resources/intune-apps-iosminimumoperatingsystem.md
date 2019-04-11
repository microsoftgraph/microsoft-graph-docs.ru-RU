---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3775a9bbc9eee6bfef5dd1bef8235bf6fc770603
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795178"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="beef1-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="beef1-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="beef1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beef1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beef1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="beef1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beef1-106">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="beef1-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="beef1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="beef1-107">Properties</span></span>
|<span data-ttu-id="beef1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="beef1-108">Property</span></span>|<span data-ttu-id="beef1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="beef1-109">Type</span></span>|<span data-ttu-id="beef1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="beef1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beef1-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="beef1-111">v8_0</span></span>|<span data-ttu-id="beef1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="beef1-112">Boolean</span></span>|<span data-ttu-id="beef1-113">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="beef1-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="beef1-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="beef1-114">v9_0</span></span>|<span data-ttu-id="beef1-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="beef1-115">Boolean</span></span>|<span data-ttu-id="beef1-116">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="beef1-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="beef1-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="beef1-117">v10_0</span></span>|<span data-ttu-id="beef1-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="beef1-118">Boolean</span></span>|<span data-ttu-id="beef1-119">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="beef1-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="beef1-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="beef1-120">v11_0</span></span>|<span data-ttu-id="beef1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="beef1-121">Boolean</span></span>|<span data-ttu-id="beef1-122">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="beef1-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="beef1-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="beef1-123">v12_0</span></span>|<span data-ttu-id="beef1-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="beef1-124">Boolean</span></span>|<span data-ttu-id="beef1-125">Версия 12,0 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="beef1-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="beef1-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="beef1-126">Relationships</span></span>
<span data-ttu-id="beef1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="beef1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="beef1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="beef1-128">JSON Representation</span></span>
<span data-ttu-id="beef1-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beef1-129">Here is a JSON representation of the resource.</span></span>
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





