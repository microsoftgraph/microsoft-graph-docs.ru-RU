---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd734d2cb7c1c03cfdab62b8a8f1acd9acac6814
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846727"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="2c39a-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="2c39a-103">rgbColor resource type</span></span>

> <span data-ttu-id="2c39a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c39a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c39a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c39a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c39a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2c39a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c39a-107">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="2c39a-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="2c39a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c39a-108">Properties</span></span>
|<span data-ttu-id="2c39a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c39a-109">Property</span></span>|<span data-ttu-id="2c39a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c39a-110">Type</span></span>|<span data-ttu-id="2c39a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c39a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c39a-112">r</span><span class="sxs-lookup"><span data-stu-id="2c39a-112">r</span></span>|<span data-ttu-id="2c39a-113">Байт</span><span class="sxs-lookup"><span data-stu-id="2c39a-113">Byte</span></span>|<span data-ttu-id="2c39a-114">Значение красного</span><span class="sxs-lookup"><span data-stu-id="2c39a-114">Red value</span></span>|
|<span data-ttu-id="2c39a-115">g</span><span class="sxs-lookup"><span data-stu-id="2c39a-115">g</span></span>|<span data-ttu-id="2c39a-116">Байт</span><span class="sxs-lookup"><span data-stu-id="2c39a-116">Byte</span></span>|<span data-ttu-id="2c39a-117">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="2c39a-117">Green value</span></span>|
|<span data-ttu-id="2c39a-118">b</span><span class="sxs-lookup"><span data-stu-id="2c39a-118">b</span></span>|<span data-ttu-id="2c39a-119">Байт</span><span class="sxs-lookup"><span data-stu-id="2c39a-119">Byte</span></span>|<span data-ttu-id="2c39a-120">Значение синего</span><span class="sxs-lookup"><span data-stu-id="2c39a-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c39a-121">Связи</span><span class="sxs-lookup"><span data-stu-id="2c39a-121">Relationships</span></span>
<span data-ttu-id="2c39a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2c39a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c39a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c39a-123">JSON Representation</span></span>
<span data-ttu-id="2c39a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c39a-124">Here is a JSON representation of the resource.</span></span>
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





