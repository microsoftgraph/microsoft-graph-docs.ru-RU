---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd61874b0b7149c718ba790b2cdee23912a0a832
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439592"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="b84f0-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b84f0-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="b84f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b84f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b84f0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b84f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b84f0-106">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="b84f0-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="b84f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b84f0-107">Properties</span></span>
|<span data-ttu-id="b84f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b84f0-108">Property</span></span>|<span data-ttu-id="b84f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b84f0-109">Type</span></span>|<span data-ttu-id="b84f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b84f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b84f0-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="b84f0-111">v8_0</span></span>|<span data-ttu-id="b84f0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b84f0-112">Boolean</span></span>|<span data-ttu-id="b84f0-113">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="b84f0-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="b84f0-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="b84f0-114">v8_1</span></span>|<span data-ttu-id="b84f0-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b84f0-115">Boolean</span></span>|<span data-ttu-id="b84f0-116">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="b84f0-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="b84f0-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="b84f0-117">v10_0</span></span>|<span data-ttu-id="b84f0-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="b84f0-118">Boolean</span></span>|<span data-ttu-id="b84f0-119">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="b84f0-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b84f0-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b84f0-120">Relationships</span></span>
<span data-ttu-id="b84f0-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b84f0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b84f0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b84f0-122">JSON Representation</span></span>
<span data-ttu-id="b84f0-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b84f0-123">Here is a JSON representation of the resource.</span></span>
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







