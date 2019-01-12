---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3593c743d0b65d761abf18b7fdb4783d126c19f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928859"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="fc35b-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="fc35b-103">rgbColor resource type</span></span>

> <span data-ttu-id="fc35b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc35b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc35b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc35b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc35b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc35b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc35b-107">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="fc35b-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="fc35b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc35b-108">Properties</span></span>
|<span data-ttu-id="fc35b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc35b-109">Property</span></span>|<span data-ttu-id="fc35b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc35b-110">Type</span></span>|<span data-ttu-id="fc35b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc35b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc35b-112">r</span><span class="sxs-lookup"><span data-stu-id="fc35b-112">r</span></span>|<span data-ttu-id="fc35b-113">Байт</span><span class="sxs-lookup"><span data-stu-id="fc35b-113">Byte</span></span>|<span data-ttu-id="fc35b-114">Значение красного</span><span class="sxs-lookup"><span data-stu-id="fc35b-114">Red value</span></span>|
|<span data-ttu-id="fc35b-115">g</span><span class="sxs-lookup"><span data-stu-id="fc35b-115">g</span></span>|<span data-ttu-id="fc35b-116">Байт</span><span class="sxs-lookup"><span data-stu-id="fc35b-116">Byte</span></span>|<span data-ttu-id="fc35b-117">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="fc35b-117">Green value</span></span>|
|<span data-ttu-id="fc35b-118">b</span><span class="sxs-lookup"><span data-stu-id="fc35b-118">b</span></span>|<span data-ttu-id="fc35b-119">Байт</span><span class="sxs-lookup"><span data-stu-id="fc35b-119">Byte</span></span>|<span data-ttu-id="fc35b-120">Значение синего</span><span class="sxs-lookup"><span data-stu-id="fc35b-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc35b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="fc35b-121">Relationships</span></span>
<span data-ttu-id="fc35b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fc35b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc35b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc35b-123">JSON Representation</span></span>
<span data-ttu-id="fc35b-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc35b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```





