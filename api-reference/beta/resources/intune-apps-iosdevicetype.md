---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
ms.openlocfilehash: 4d85d8801934e6f240bacd6fafe63c7bd1ee946f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078818"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="8681a-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8681a-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="8681a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8681a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8681a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8681a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8681a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8681a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8681a-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="8681a-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="8681a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8681a-108">Properties</span></span>
|<span data-ttu-id="8681a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8681a-109">Property</span></span>|<span data-ttu-id="8681a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8681a-110">Type</span></span>|<span data-ttu-id="8681a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8681a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8681a-112">iPad</span><span class="sxs-lookup"><span data-stu-id="8681a-112">iPad</span></span>|<span data-ttu-id="8681a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8681a-113">Boolean</span></span>|<span data-ttu-id="8681a-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="8681a-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="8681a-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="8681a-115">iPhoneAndIPod</span></span>|<span data-ttu-id="8681a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8681a-116">Boolean</span></span>|<span data-ttu-id="8681a-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="8681a-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8681a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8681a-118">Relationships</span></span>
<span data-ttu-id="8681a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8681a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8681a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8681a-120">JSON Representation</span></span>
<span data-ttu-id="8681a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8681a-121">Here is a JSON representation of the resource.</span></span>
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





