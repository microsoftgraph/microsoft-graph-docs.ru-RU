---
title: Тип ресурса iosDeviceType
description: Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fe1f686052468bbab5d7115541a631b77073d6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977166"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="71513-103">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="71513-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="71513-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71513-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71513-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71513-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71513-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71513-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71513-107">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="71513-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="71513-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="71513-108">Properties</span></span>
|<span data-ttu-id="71513-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="71513-109">Property</span></span>|<span data-ttu-id="71513-110">Тип</span><span class="sxs-lookup"><span data-stu-id="71513-110">Type</span></span>|<span data-ttu-id="71513-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71513-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71513-112">iPad</span><span class="sxs-lookup"><span data-stu-id="71513-112">iPad</span></span>|<span data-ttu-id="71513-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="71513-113">Boolean</span></span>|<span data-ttu-id="71513-114">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="71513-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="71513-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="71513-115">iPhoneAndIPod</span></span>|<span data-ttu-id="71513-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="71513-116">Boolean</span></span>|<span data-ttu-id="71513-117">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="71513-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71513-118">Связи</span><span class="sxs-lookup"><span data-stu-id="71513-118">Relationships</span></span>
<span data-ttu-id="71513-119">Нет</span><span class="sxs-lookup"><span data-stu-id="71513-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71513-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71513-120">JSON Representation</span></span>
<span data-ttu-id="71513-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71513-121">Here is a JSON representation of the resource.</span></span>
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





