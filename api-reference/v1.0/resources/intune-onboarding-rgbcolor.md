---
title: Тип ресурса rgbColor
description: Цвет в формате RGB.
ms.openlocfilehash: 5b3ef1f7b26925721098f82ec2bf54c614ce399b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028362"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="37d52-103">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="37d52-103">rgbColor resource type</span></span>

> <span data-ttu-id="37d52-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="37d52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37d52-105">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="37d52-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="37d52-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="37d52-106">Properties</span></span>
|<span data-ttu-id="37d52-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d52-107">Property</span></span>|<span data-ttu-id="37d52-108">Тип</span><span class="sxs-lookup"><span data-stu-id="37d52-108">Type</span></span>|<span data-ttu-id="37d52-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37d52-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d52-110">r</span><span class="sxs-lookup"><span data-stu-id="37d52-110">r</span></span>|<span data-ttu-id="37d52-111">Байт</span><span class="sxs-lookup"><span data-stu-id="37d52-111">Byte</span></span>|<span data-ttu-id="37d52-112">Значение красного</span><span class="sxs-lookup"><span data-stu-id="37d52-112">Red value</span></span>|
|<span data-ttu-id="37d52-113">g</span><span class="sxs-lookup"><span data-stu-id="37d52-113">g</span></span>|<span data-ttu-id="37d52-114">Байт</span><span class="sxs-lookup"><span data-stu-id="37d52-114">Byte</span></span>|<span data-ttu-id="37d52-115">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="37d52-115">Green value</span></span>|
|<span data-ttu-id="37d52-116">b</span><span class="sxs-lookup"><span data-stu-id="37d52-116">b</span></span>|<span data-ttu-id="37d52-117">Байт</span><span class="sxs-lookup"><span data-stu-id="37d52-117">Byte</span></span>|<span data-ttu-id="37d52-118">Значение синего</span><span class="sxs-lookup"><span data-stu-id="37d52-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="37d52-119">Связи</span><span class="sxs-lookup"><span data-stu-id="37d52-119">Relationships</span></span>
<span data-ttu-id="37d52-120">Нет</span><span class="sxs-lookup"><span data-stu-id="37d52-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37d52-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37d52-121">JSON Representation</span></span>
<span data-ttu-id="37d52-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37d52-122">Here is a JSON representation of the resource.</span></span>
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



