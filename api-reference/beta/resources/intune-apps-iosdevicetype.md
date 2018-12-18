---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
ms.openlocfilehash: c9f691c2fdeb25bad54c105450c71dd7c65f30b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342758"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="3225d-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3225d-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="3225d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3225d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3225d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3225d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3225d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3225d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3225d-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="3225d-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="3225d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3225d-108">Properties</span></span>
|<span data-ttu-id="3225d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3225d-109">Property</span></span>|<span data-ttu-id="3225d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3225d-110">Type</span></span>|<span data-ttu-id="3225d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3225d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3225d-112">iPad</span><span class="sxs-lookup"><span data-stu-id="3225d-112">iPad</span></span>|<span data-ttu-id="3225d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="3225d-113">Boolean</span></span>|<span data-ttu-id="3225d-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="3225d-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="3225d-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="3225d-115">iPhoneAndIPod</span></span>|<span data-ttu-id="3225d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3225d-116">Boolean</span></span>|<span data-ttu-id="3225d-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="3225d-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3225d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3225d-118">Relationships</span></span>
<span data-ttu-id="3225d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3225d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3225d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3225d-120">JSON Representation</span></span>
<span data-ttu-id="3225d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3225d-121">Here is a JSON representation of the resource.</span></span>
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





