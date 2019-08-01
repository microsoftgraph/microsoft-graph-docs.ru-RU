---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da56780e66e88baaa074c3106997e3b4a3cc3b64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032349"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="c930c-103">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c930c-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="c930c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c930c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c930c-105">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="c930c-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="c930c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c930c-106">Properties</span></span>
|<span data-ttu-id="c930c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c930c-107">Property</span></span>|<span data-ttu-id="c930c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c930c-108">Type</span></span>|<span data-ttu-id="c930c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c930c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c930c-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="c930c-110">v8_0</span></span>|<span data-ttu-id="c930c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="c930c-111">Boolean</span></span>|<span data-ttu-id="c930c-112">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c930c-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="c930c-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="c930c-113">v9_0</span></span>|<span data-ttu-id="c930c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c930c-114">Boolean</span></span>|<span data-ttu-id="c930c-115">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c930c-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="c930c-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="c930c-116">v10_0</span></span>|<span data-ttu-id="c930c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c930c-117">Boolean</span></span>|<span data-ttu-id="c930c-118">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c930c-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="c930c-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="c930c-119">v11_0</span></span>|<span data-ttu-id="c930c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c930c-120">Boolean</span></span>|<span data-ttu-id="c930c-121">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="c930c-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="c930c-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="c930c-122">v12_0</span></span>|<span data-ttu-id="c930c-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="c930c-123">Boolean</span></span>|<span data-ttu-id="c930c-124">Версия 12,0 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="c930c-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c930c-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="c930c-125">Relationships</span></span>
<span data-ttu-id="c930c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c930c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c930c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c930c-127">JSON Representation</span></span>
<span data-ttu-id="c930c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c930c-128">Here is a JSON representation of the resource.</span></span>
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



