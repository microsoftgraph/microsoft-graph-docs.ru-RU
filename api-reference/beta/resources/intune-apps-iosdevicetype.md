---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d475b129fa74439c1d5876b96579d556540177f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884884"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="3b238-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3b238-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="3b238-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b238-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b238-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b238-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b238-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b238-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b238-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="3b238-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="3b238-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b238-108">Properties</span></span>
|<span data-ttu-id="3b238-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b238-109">Property</span></span>|<span data-ttu-id="3b238-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3b238-110">Type</span></span>|<span data-ttu-id="3b238-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3b238-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b238-112">iPad</span><span class="sxs-lookup"><span data-stu-id="3b238-112">iPad</span></span>|<span data-ttu-id="3b238-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b238-113">Boolean</span></span>|<span data-ttu-id="3b238-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="3b238-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="3b238-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="3b238-115">iPhoneAndIPod</span></span>|<span data-ttu-id="3b238-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b238-116">Boolean</span></span>|<span data-ttu-id="3b238-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="3b238-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b238-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3b238-118">Relationships</span></span>
<span data-ttu-id="3b238-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3b238-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b238-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b238-120">JSON Representation</span></span>
<span data-ttu-id="3b238-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b238-121">Here is a JSON representation of the resource.</span></span>
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





