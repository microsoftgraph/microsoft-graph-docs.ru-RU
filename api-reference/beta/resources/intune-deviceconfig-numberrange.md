---
title: Тип ресурса numberRange
description: Определение номер диапазона.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27393bdac6519078c2021e3484ae58ddf43216d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416862"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="43ff3-103">Тип ресурса numberRange</span><span class="sxs-lookup"><span data-stu-id="43ff3-103">numberRange resource type</span></span>

> <span data-ttu-id="43ff3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43ff3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43ff3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43ff3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43ff3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43ff3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43ff3-107">Определение номер диапазона.</span><span class="sxs-lookup"><span data-stu-id="43ff3-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="43ff3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="43ff3-108">Properties</span></span>
|<span data-ttu-id="43ff3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="43ff3-109">Property</span></span>|<span data-ttu-id="43ff3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="43ff3-110">Type</span></span>|<span data-ttu-id="43ff3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="43ff3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43ff3-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="43ff3-112">lowerNumber</span></span>|<span data-ttu-id="43ff3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="43ff3-113">Int32</span></span>|<span data-ttu-id="43ff3-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="43ff3-114">Lower number.</span></span>|
|<span data-ttu-id="43ff3-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="43ff3-115">upperNumber</span></span>|<span data-ttu-id="43ff3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="43ff3-116">Int32</span></span>|<span data-ttu-id="43ff3-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="43ff3-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43ff3-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="43ff3-118">Relationships</span></span>
<span data-ttu-id="43ff3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="43ff3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43ff3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43ff3-120">JSON Representation</span></span>
<span data-ttu-id="43ff3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43ff3-121">Here is a JSON representation of the resource.</span></span>
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




