---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
ms.openlocfilehash: b14abbb6713daf9fad7b0d2fd6f7865d251b6147
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026409"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e470e-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e470e-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="e470e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e470e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e470e-105">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="e470e-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="e470e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e470e-106">Properties</span></span>
|<span data-ttu-id="e470e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e470e-107">Property</span></span>|<span data-ttu-id="e470e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e470e-108">Type</span></span>|<span data-ttu-id="e470e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e470e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e470e-110">iPad</span><span class="sxs-lookup"><span data-stu-id="e470e-110">iPad</span></span>|<span data-ttu-id="e470e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e470e-111">Boolean</span></span>|<span data-ttu-id="e470e-112">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="e470e-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e470e-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e470e-113">iPhoneAndIPod</span></span>|<span data-ttu-id="e470e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e470e-114">Boolean</span></span>|<span data-ttu-id="e470e-115">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="e470e-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e470e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="e470e-116">Relationships</span></span>
<span data-ttu-id="e470e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e470e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e470e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e470e-118">JSON Representation</span></span>
<span data-ttu-id="e470e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e470e-119">Here is a JSON representation of the resource.</span></span>
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



