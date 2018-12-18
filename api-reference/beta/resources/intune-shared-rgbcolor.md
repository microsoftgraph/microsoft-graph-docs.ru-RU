---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
author: tfitzmac
ms.openlocfilehash: 0452d8c275e7568df6b304613d8619f04add0548
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307114"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="b2b87-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="b2b87-103">rgbColor resource type</span></span>

> <span data-ttu-id="b2b87-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2b87-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2b87-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2b87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2b87-107">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="b2b87-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="b2b87-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2b87-108">Properties</span></span>
|<span data-ttu-id="b2b87-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2b87-109">Property</span></span>|<span data-ttu-id="b2b87-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2b87-110">Type</span></span>|<span data-ttu-id="b2b87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b87-112">r</span><span class="sxs-lookup"><span data-stu-id="b2b87-112">r</span></span>|<span data-ttu-id="b2b87-113">Байт</span><span class="sxs-lookup"><span data-stu-id="b2b87-113">Byte</span></span>|<span data-ttu-id="b2b87-114">Значение красного</span><span class="sxs-lookup"><span data-stu-id="b2b87-114">Red value</span></span>|
|<span data-ttu-id="b2b87-115">g</span><span class="sxs-lookup"><span data-stu-id="b2b87-115">g</span></span>|<span data-ttu-id="b2b87-116">Байт</span><span class="sxs-lookup"><span data-stu-id="b2b87-116">Byte</span></span>|<span data-ttu-id="b2b87-117">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="b2b87-117">Green value</span></span>|
|<span data-ttu-id="b2b87-118">b</span><span class="sxs-lookup"><span data-stu-id="b2b87-118">b</span></span>|<span data-ttu-id="b2b87-119">Байт</span><span class="sxs-lookup"><span data-stu-id="b2b87-119">Byte</span></span>|<span data-ttu-id="b2b87-120">Значение синего</span><span class="sxs-lookup"><span data-stu-id="b2b87-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2b87-121">Связи</span><span class="sxs-lookup"><span data-stu-id="b2b87-121">Relationships</span></span>
<span data-ttu-id="b2b87-122">Нет</span><span class="sxs-lookup"><span data-stu-id="b2b87-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2b87-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2b87-123">JSON Representation</span></span>
<span data-ttu-id="b2b87-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2b87-124">Here is a JSON representation of the resource.</span></span>
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





