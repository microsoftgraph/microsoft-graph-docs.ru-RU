---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
author: tfitzmac
ms.openlocfilehash: b469533b8ee7e54e99b09be08870045d759f5322
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350962"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="cb150-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="cb150-103">rgbColor resource type</span></span>

> <span data-ttu-id="cb150-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb150-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb150-105">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="cb150-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="cb150-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb150-106">Properties</span></span>
|<span data-ttu-id="cb150-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb150-107">Property</span></span>|<span data-ttu-id="cb150-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb150-108">Type</span></span>|<span data-ttu-id="cb150-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb150-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb150-110">r</span><span class="sxs-lookup"><span data-stu-id="cb150-110">r</span></span>|<span data-ttu-id="cb150-111">Байт</span><span class="sxs-lookup"><span data-stu-id="cb150-111">Byte</span></span>|<span data-ttu-id="cb150-112">Значение красного</span><span class="sxs-lookup"><span data-stu-id="cb150-112">Red value</span></span>|
|<span data-ttu-id="cb150-113">g</span><span class="sxs-lookup"><span data-stu-id="cb150-113">g</span></span>|<span data-ttu-id="cb150-114">Байт</span><span class="sxs-lookup"><span data-stu-id="cb150-114">Byte</span></span>|<span data-ttu-id="cb150-115">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="cb150-115">Green value</span></span>|
|<span data-ttu-id="cb150-116">b</span><span class="sxs-lookup"><span data-stu-id="cb150-116">b</span></span>|<span data-ttu-id="cb150-117">Байт</span><span class="sxs-lookup"><span data-stu-id="cb150-117">Byte</span></span>|<span data-ttu-id="cb150-118">Значение синего</span><span class="sxs-lookup"><span data-stu-id="cb150-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb150-119">Связи</span><span class="sxs-lookup"><span data-stu-id="cb150-119">Relationships</span></span>
<span data-ttu-id="cb150-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cb150-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb150-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb150-121">JSON Representation</span></span>
<span data-ttu-id="cb150-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb150-122">Here is a JSON representation of the resource.</span></span>
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



