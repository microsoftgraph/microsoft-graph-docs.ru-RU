---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523884"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="1d042-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1d042-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="1d042-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d042-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d042-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="1d042-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="1d042-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d042-106">Properties</span></span>
|<span data-ttu-id="1d042-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d042-107">Property</span></span>|<span data-ttu-id="1d042-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1d042-108">Type</span></span>|<span data-ttu-id="1d042-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1d042-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d042-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="1d042-110">v8_0</span></span>|<span data-ttu-id="1d042-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d042-111">Boolean</span></span>|<span data-ttu-id="1d042-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="1d042-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="1d042-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="1d042-113">v9_0</span></span>|<span data-ttu-id="1d042-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d042-114">Boolean</span></span>|<span data-ttu-id="1d042-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="1d042-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="1d042-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="1d042-116">v10_0</span></span>|<span data-ttu-id="1d042-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d042-117">Boolean</span></span>|<span data-ttu-id="1d042-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="1d042-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="1d042-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="1d042-119">v11_0</span></span>|<span data-ttu-id="1d042-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d042-120">Boolean</span></span>|<span data-ttu-id="1d042-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="1d042-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="1d042-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="1d042-122">v12_0</span></span>|<span data-ttu-id="1d042-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d042-123">Boolean</span></span>|<span data-ttu-id="1d042-124">Версия 12,0 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="1d042-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d042-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d042-125">Relationships</span></span>
<span data-ttu-id="1d042-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1d042-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d042-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d042-127">JSON Representation</span></span>
<span data-ttu-id="1d042-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d042-128">Here is a JSON representation of the resource.</span></span>
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



