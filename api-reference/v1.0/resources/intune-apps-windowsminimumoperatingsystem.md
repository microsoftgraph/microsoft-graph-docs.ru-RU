---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 574ca504ec7b0cd736735323e534bfd3ed17f31b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755982"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="2cd1b-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2cd1b-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="2cd1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cd1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cd1b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd1b-106">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="2cd1b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cd1b-107">Properties</span></span>
|<span data-ttu-id="2cd1b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cd1b-108">Property</span></span>|<span data-ttu-id="2cd1b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2cd1b-109">Type</span></span>|<span data-ttu-id="2cd1b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2cd1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd1b-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="2cd1b-111">v8_0</span></span>|<span data-ttu-id="2cd1b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1b-112">Boolean</span></span>|<span data-ttu-id="2cd1b-113">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="2cd1b-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="2cd1b-114">v8_1</span></span>|<span data-ttu-id="2cd1b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1b-115">Boolean</span></span>|<span data-ttu-id="2cd1b-116">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="2cd1b-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="2cd1b-117">v10_0</span></span>|<span data-ttu-id="2cd1b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1b-118">Boolean</span></span>|<span data-ttu-id="2cd1b-119">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd1b-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="2cd1b-120">Relationships</span></span>
<span data-ttu-id="2cd1b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2cd1b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cd1b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cd1b-122">JSON Representation</span></span>
<span data-ttu-id="2cd1b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cd1b-123">Here is a JSON representation of the resource.</span></span>
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




