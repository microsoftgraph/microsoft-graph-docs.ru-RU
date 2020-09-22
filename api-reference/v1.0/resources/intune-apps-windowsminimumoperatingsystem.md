---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9f9dc76e287e6533b2b33606825a19da67d8675
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032490"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="58e42-103">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58e42-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="58e42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58e42-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58e42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58e42-106">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="58e42-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="58e42-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58e42-107">Properties</span></span>
|<span data-ttu-id="58e42-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="58e42-108">Property</span></span>|<span data-ttu-id="58e42-109">Тип</span><span class="sxs-lookup"><span data-stu-id="58e42-109">Type</span></span>|<span data-ttu-id="58e42-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58e42-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58e42-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="58e42-111">v8_0</span></span>|<span data-ttu-id="58e42-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e42-112">Boolean</span></span>|<span data-ttu-id="58e42-113">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="58e42-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="58e42-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="58e42-114">v8_1</span></span>|<span data-ttu-id="58e42-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e42-115">Boolean</span></span>|<span data-ttu-id="58e42-116">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="58e42-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="58e42-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="58e42-117">v10_0</span></span>|<span data-ttu-id="58e42-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e42-118">Boolean</span></span>|<span data-ttu-id="58e42-119">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="58e42-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58e42-120">Связи</span><span class="sxs-lookup"><span data-stu-id="58e42-120">Relationships</span></span>
<span data-ttu-id="58e42-121">Нет</span><span class="sxs-lookup"><span data-stu-id="58e42-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58e42-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58e42-122">JSON Representation</span></span>
<span data-ttu-id="58e42-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58e42-123">Here is a JSON representation of the resource.</span></span>
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









