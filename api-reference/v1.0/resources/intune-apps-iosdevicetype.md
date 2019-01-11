---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ffa46d1e8fb693822051250fb4a722815b1dcb73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866782"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="2f588-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2f588-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="2f588-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f588-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f588-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="2f588-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="2f588-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f588-106">Properties</span></span>
|<span data-ttu-id="2f588-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f588-107">Property</span></span>|<span data-ttu-id="2f588-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f588-108">Type</span></span>|<span data-ttu-id="2f588-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f588-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f588-110">iPad</span><span class="sxs-lookup"><span data-stu-id="2f588-110">iPad</span></span>|<span data-ttu-id="2f588-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f588-111">Boolean</span></span>|<span data-ttu-id="2f588-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="2f588-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="2f588-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="2f588-113">iPhoneAndIPod</span></span>|<span data-ttu-id="2f588-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f588-114">Boolean</span></span>|<span data-ttu-id="2f588-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="2f588-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f588-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2f588-116">Relationships</span></span>
<span data-ttu-id="2f588-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2f588-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f588-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f588-118">JSON Representation</span></span>
<span data-ttu-id="2f588-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f588-119">Here is a JSON representation of the resource.</span></span>
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



