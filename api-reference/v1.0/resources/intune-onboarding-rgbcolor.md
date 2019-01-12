---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc40b5cc2ffff02bed89847386db6398f76b3953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967009"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="b821f-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="b821f-103">rgbColor resource type</span></span>

> <span data-ttu-id="b821f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b821f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b821f-105">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="b821f-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="b821f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b821f-106">Properties</span></span>
|<span data-ttu-id="b821f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b821f-107">Property</span></span>|<span data-ttu-id="b821f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b821f-108">Type</span></span>|<span data-ttu-id="b821f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b821f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b821f-110">r</span><span class="sxs-lookup"><span data-stu-id="b821f-110">r</span></span>|<span data-ttu-id="b821f-111">Байт</span><span class="sxs-lookup"><span data-stu-id="b821f-111">Byte</span></span>|<span data-ttu-id="b821f-112">Значение красного</span><span class="sxs-lookup"><span data-stu-id="b821f-112">Red value</span></span>|
|<span data-ttu-id="b821f-113">g</span><span class="sxs-lookup"><span data-stu-id="b821f-113">g</span></span>|<span data-ttu-id="b821f-114">Байт</span><span class="sxs-lookup"><span data-stu-id="b821f-114">Byte</span></span>|<span data-ttu-id="b821f-115">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="b821f-115">Green value</span></span>|
|<span data-ttu-id="b821f-116">b</span><span class="sxs-lookup"><span data-stu-id="b821f-116">b</span></span>|<span data-ttu-id="b821f-117">Байт</span><span class="sxs-lookup"><span data-stu-id="b821f-117">Byte</span></span>|<span data-ttu-id="b821f-118">Значение синего</span><span class="sxs-lookup"><span data-stu-id="b821f-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b821f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b821f-119">Relationships</span></span>
<span data-ttu-id="b821f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b821f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b821f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b821f-121">JSON Representation</span></span>
<span data-ttu-id="b821f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b821f-122">Here is a JSON representation of the resource.</span></span>
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



