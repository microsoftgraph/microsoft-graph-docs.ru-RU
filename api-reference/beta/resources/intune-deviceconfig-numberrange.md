---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166789"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="4fe4d-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="4fe4d-103">numberRange resource type</span></span>

> <span data-ttu-id="4fe4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fe4d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe4d-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="4fe4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fe4d-107">Properties</span></span>
|<span data-ttu-id="4fe4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fe4d-108">Property</span></span>|<span data-ttu-id="4fe4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4fe4d-109">Type</span></span>|<span data-ttu-id="4fe4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4fe4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fe4d-111">Ловернумбер</span><span class="sxs-lookup"><span data-stu-id="4fe4d-111">lowerNumber</span></span>|<span data-ttu-id="4fe4d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4fe4d-112">Int32</span></span>|<span data-ttu-id="4fe4d-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-113">Lower number.</span></span>|
|<span data-ttu-id="4fe4d-114">Уппернумбер</span><span class="sxs-lookup"><span data-stu-id="4fe4d-114">upperNumber</span></span>|<span data-ttu-id="4fe4d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="4fe4d-115">Int32</span></span>|<span data-ttu-id="4fe4d-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fe4d-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="4fe4d-117">Relationships</span></span>
<span data-ttu-id="4fe4d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4fe4d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fe4d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fe4d-119">JSON Representation</span></span>
<span data-ttu-id="4fe4d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe4d-120">Here is a JSON representation of the resource.</span></span>
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




