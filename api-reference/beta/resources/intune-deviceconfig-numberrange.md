---
title: Тип ресурса numberRange
description: Определение номер диапазона.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b428320fd66263149b6d443a15c6a0e1eee744a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845705"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="992c6-103">Тип ресурса numberRange</span><span class="sxs-lookup"><span data-stu-id="992c6-103">numberRange resource type</span></span>

> <span data-ttu-id="992c6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="992c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="992c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="992c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="992c6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="992c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="992c6-107">Определение номер диапазона.</span><span class="sxs-lookup"><span data-stu-id="992c6-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="992c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="992c6-108">Properties</span></span>
|<span data-ttu-id="992c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="992c6-109">Property</span></span>|<span data-ttu-id="992c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="992c6-110">Type</span></span>|<span data-ttu-id="992c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="992c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="992c6-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="992c6-112">lowerNumber</span></span>|<span data-ttu-id="992c6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="992c6-113">Int32</span></span>|<span data-ttu-id="992c6-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="992c6-114">Lower number.</span></span>|
|<span data-ttu-id="992c6-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="992c6-115">upperNumber</span></span>|<span data-ttu-id="992c6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="992c6-116">Int32</span></span>|<span data-ttu-id="992c6-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="992c6-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="992c6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="992c6-118">Relationships</span></span>
<span data-ttu-id="992c6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="992c6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="992c6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="992c6-120">JSON Representation</span></span>
<span data-ttu-id="992c6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="992c6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





