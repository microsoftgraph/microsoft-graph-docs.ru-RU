---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
ms.openlocfilehash: 7b5d450c0126e043a78a6c4f9f0e2fe6f06c7c13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080628"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="f5a60-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="f5a60-103">rgbColor resource type</span></span>

> <span data-ttu-id="f5a60-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5a60-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5a60-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5a60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5a60-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f5a60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5a60-107">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="f5a60-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="f5a60-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5a60-108">Properties</span></span>
|<span data-ttu-id="f5a60-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5a60-109">Property</span></span>|<span data-ttu-id="f5a60-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5a60-110">Type</span></span>|<span data-ttu-id="f5a60-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5a60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5a60-112">r</span><span class="sxs-lookup"><span data-stu-id="f5a60-112">r</span></span>|<span data-ttu-id="f5a60-113">Байт</span><span class="sxs-lookup"><span data-stu-id="f5a60-113">Byte</span></span>|<span data-ttu-id="f5a60-114">Значение красного</span><span class="sxs-lookup"><span data-stu-id="f5a60-114">Red value</span></span>|
|<span data-ttu-id="f5a60-115">g</span><span class="sxs-lookup"><span data-stu-id="f5a60-115">g</span></span>|<span data-ttu-id="f5a60-116">Байт</span><span class="sxs-lookup"><span data-stu-id="f5a60-116">Byte</span></span>|<span data-ttu-id="f5a60-117">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="f5a60-117">Green value</span></span>|
|<span data-ttu-id="f5a60-118">b</span><span class="sxs-lookup"><span data-stu-id="f5a60-118">b</span></span>|<span data-ttu-id="f5a60-119">Байт</span><span class="sxs-lookup"><span data-stu-id="f5a60-119">Byte</span></span>|<span data-ttu-id="f5a60-120">Значение синего</span><span class="sxs-lookup"><span data-stu-id="f5a60-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5a60-121">Связи</span><span class="sxs-lookup"><span data-stu-id="f5a60-121">Relationships</span></span>
<span data-ttu-id="f5a60-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f5a60-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5a60-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5a60-123">JSON Representation</span></span>
<span data-ttu-id="f5a60-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5a60-124">Here is a JSON representation of the resource.</span></span>
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





