---
title: Тип ресурса numberRange
description: Определение номер диапазона.
author: tfitzmac
ms.openlocfilehash: 7b9703524e1562a7367a3c5b9bf0212e29620429
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314660"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="44c28-103">Тип ресурса numberRange</span><span class="sxs-lookup"><span data-stu-id="44c28-103">numberRange resource type</span></span>

> <span data-ttu-id="44c28-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44c28-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44c28-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44c28-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44c28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44c28-107">Определение номер диапазона.</span><span class="sxs-lookup"><span data-stu-id="44c28-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="44c28-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44c28-108">Properties</span></span>
|<span data-ttu-id="44c28-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44c28-109">Property</span></span>|<span data-ttu-id="44c28-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44c28-110">Type</span></span>|<span data-ttu-id="44c28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44c28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c28-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="44c28-112">lowerNumber</span></span>|<span data-ttu-id="44c28-113">Int32</span><span class="sxs-lookup"><span data-stu-id="44c28-113">Int32</span></span>|<span data-ttu-id="44c28-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="44c28-114">Lower number.</span></span>|
|<span data-ttu-id="44c28-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="44c28-115">upperNumber</span></span>|<span data-ttu-id="44c28-116">Int32</span><span class="sxs-lookup"><span data-stu-id="44c28-116">Int32</span></span>|<span data-ttu-id="44c28-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="44c28-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44c28-118">Связи</span><span class="sxs-lookup"><span data-stu-id="44c28-118">Relationships</span></span>
<span data-ttu-id="44c28-119">Нет</span><span class="sxs-lookup"><span data-stu-id="44c28-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44c28-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44c28-120">JSON Representation</span></span>
<span data-ttu-id="44c28-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44c28-121">Here is a JSON representation of the resource.</span></span>
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





