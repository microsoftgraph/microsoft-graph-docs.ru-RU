---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a92d02f6994a7cd18ba44c7da5b43768e87fc61a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032077"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="369b3-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="369b3-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="369b3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="369b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369b3-105">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="369b3-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="369b3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="369b3-106">Properties</span></span>
|<span data-ttu-id="369b3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="369b3-107">Property</span></span>|<span data-ttu-id="369b3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="369b3-108">Type</span></span>|<span data-ttu-id="369b3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="369b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="369b3-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="369b3-110">v8_0</span></span>|<span data-ttu-id="369b3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="369b3-111">Boolean</span></span>|<span data-ttu-id="369b3-112">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="369b3-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="369b3-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="369b3-113">v8_1</span></span>|<span data-ttu-id="369b3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="369b3-114">Boolean</span></span>|<span data-ttu-id="369b3-115">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="369b3-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="369b3-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="369b3-116">v10_0</span></span>|<span data-ttu-id="369b3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="369b3-117">Boolean</span></span>|<span data-ttu-id="369b3-118">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="369b3-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="369b3-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="369b3-119">Relationships</span></span>
<span data-ttu-id="369b3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="369b3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="369b3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="369b3-121">JSON Representation</span></span>
<span data-ttu-id="369b3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="369b3-122">Here is a JSON representation of the resource.</span></span>
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



