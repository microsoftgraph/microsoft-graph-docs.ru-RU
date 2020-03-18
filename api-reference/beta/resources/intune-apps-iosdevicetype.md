---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c842d27d3113210d96479388d2395b24dea8f123
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798128"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e79a1-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e79a1-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="e79a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e79a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e79a1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e79a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79a1-106">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="e79a1-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="e79a1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e79a1-107">Properties</span></span>
|<span data-ttu-id="e79a1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e79a1-108">Property</span></span>|<span data-ttu-id="e79a1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e79a1-109">Type</span></span>|<span data-ttu-id="e79a1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e79a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79a1-111">iPad</span><span class="sxs-lookup"><span data-stu-id="e79a1-111">iPad</span></span>|<span data-ttu-id="e79a1-112">Логический</span><span class="sxs-lookup"><span data-stu-id="e79a1-112">Boolean</span></span>|<span data-ttu-id="e79a1-113">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="e79a1-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e79a1-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e79a1-114">iPhoneAndIPod</span></span>|<span data-ttu-id="e79a1-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79a1-115">Boolean</span></span>|<span data-ttu-id="e79a1-116">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="e79a1-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e79a1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="e79a1-117">Relationships</span></span>
<span data-ttu-id="e79a1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e79a1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e79a1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e79a1-119">JSON Representation</span></span>
<span data-ttu-id="e79a1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e79a1-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



