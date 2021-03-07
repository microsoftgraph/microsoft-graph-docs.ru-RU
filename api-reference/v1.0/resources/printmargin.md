---
title: тип ресурса printMargin
description: Указывает ширину поля, используемую при печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1680cc641da02f3339dcd75977c411d3255cf037
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518060"
---
# <a name="printmargin-resource-type"></a><span data-ttu-id="0d5e8-103">тип ресурса printMargin</span><span class="sxs-lookup"><span data-stu-id="0d5e8-103">printMargin resource type</span></span>

<span data-ttu-id="0d5e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d5e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0d5e8-105">Указывает ширину поля, используемую при печати.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="0d5e8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d5e8-106">Properties</span></span>
|<span data-ttu-id="0d5e8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d5e8-107">Property</span></span>|<span data-ttu-id="0d5e8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d5e8-108">Type</span></span>|<span data-ttu-id="0d5e8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d5e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d5e8-110">top</span><span class="sxs-lookup"><span data-stu-id="0d5e8-110">top</span></span>|<span data-ttu-id="0d5e8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="0d5e8-111">Int32</span></span>|<span data-ttu-id="0d5e8-112">Маржа в микронах от верхнего края.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="0d5e8-113">bottom</span><span class="sxs-lookup"><span data-stu-id="0d5e8-113">bottom</span></span>|<span data-ttu-id="0d5e8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0d5e8-114">Int32</span></span>|<span data-ttu-id="0d5e8-115">Маржа в микронах с нижнего края.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="0d5e8-116">Правильно</span><span class="sxs-lookup"><span data-stu-id="0d5e8-116">right</span></span>|<span data-ttu-id="0d5e8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0d5e8-117">Int32</span></span>|<span data-ttu-id="0d5e8-118">Поле в микронах с правого края.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="0d5e8-119">left</span><span class="sxs-lookup"><span data-stu-id="0d5e8-119">left</span></span>|<span data-ttu-id="0d5e8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0d5e8-120">Int32</span></span>|<span data-ttu-id="0d5e8-121">Поле в микронах с левого края.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d5e8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d5e8-122">JSON representation</span></span>
<span data-ttu-id="0d5e8-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d5e8-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

