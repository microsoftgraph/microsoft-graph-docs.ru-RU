---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a62cb711b70352d98650ae03945316de9ed2b5d2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356259"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="7f169-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7f169-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="7f169-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f169-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f169-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="7f169-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="7f169-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f169-106">Properties</span></span>
|<span data-ttu-id="7f169-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f169-107">Property</span></span>|<span data-ttu-id="7f169-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7f169-108">Type</span></span>|<span data-ttu-id="7f169-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f169-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f169-110">iPad</span><span class="sxs-lookup"><span data-stu-id="7f169-110">iPad</span></span>|<span data-ttu-id="7f169-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f169-111">Boolean</span></span>|<span data-ttu-id="7f169-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="7f169-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="7f169-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="7f169-113">iPhoneAndIPod</span></span>|<span data-ttu-id="7f169-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f169-114">Boolean</span></span>|<span data-ttu-id="7f169-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="7f169-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f169-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7f169-116">Relationships</span></span>
<span data-ttu-id="7f169-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7f169-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f169-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f169-118">JSON Representation</span></span>
<span data-ttu-id="7f169-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f169-119">Here is a JSON representation of the resource.</span></span>
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




