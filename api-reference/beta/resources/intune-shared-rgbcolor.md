---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 505383227d1014f779cb558d43c18da29d3989aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395519"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="2c425-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="2c425-103">rgbColor resource type</span></span>

> <span data-ttu-id="2c425-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c425-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c425-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c425-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c425-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c425-107">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="2c425-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="2c425-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c425-108">Properties</span></span>
|<span data-ttu-id="2c425-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c425-109">Property</span></span>|<span data-ttu-id="2c425-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c425-110">Type</span></span>|<span data-ttu-id="2c425-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c425-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c425-112">r</span><span class="sxs-lookup"><span data-stu-id="2c425-112">r</span></span>|<span data-ttu-id="2c425-113">Байт</span><span class="sxs-lookup"><span data-stu-id="2c425-113">Byte</span></span>|<span data-ttu-id="2c425-114">Значение красного</span><span class="sxs-lookup"><span data-stu-id="2c425-114">Red value</span></span>|
|<span data-ttu-id="2c425-115">g</span><span class="sxs-lookup"><span data-stu-id="2c425-115">g</span></span>|<span data-ttu-id="2c425-116">Байт</span><span class="sxs-lookup"><span data-stu-id="2c425-116">Byte</span></span>|<span data-ttu-id="2c425-117">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="2c425-117">Green value</span></span>|
|<span data-ttu-id="2c425-118">b</span><span class="sxs-lookup"><span data-stu-id="2c425-118">b</span></span>|<span data-ttu-id="2c425-119">Байт</span><span class="sxs-lookup"><span data-stu-id="2c425-119">Byte</span></span>|<span data-ttu-id="2c425-120">Значение синего</span><span class="sxs-lookup"><span data-stu-id="2c425-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c425-121">Связи</span><span class="sxs-lookup"><span data-stu-id="2c425-121">Relationships</span></span>
<span data-ttu-id="2c425-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2c425-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c425-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c425-123">JSON Representation</span></span>
<span data-ttu-id="2c425-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c425-124">Here is a JSON representation of the resource.</span></span>
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




