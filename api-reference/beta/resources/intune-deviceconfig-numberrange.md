---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 772ffc59bc9ac4848b6b34eee8c62f8006468784
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958720"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="b699b-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="b699b-103">numberRange resource type</span></span>

> <span data-ttu-id="b699b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b699b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b699b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b699b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b699b-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="b699b-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b699b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b699b-107">Properties</span></span>
|<span data-ttu-id="b699b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b699b-108">Property</span></span>|<span data-ttu-id="b699b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b699b-109">Type</span></span>|<span data-ttu-id="b699b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b699b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b699b-111">Ловернумбер</span><span class="sxs-lookup"><span data-stu-id="b699b-111">lowerNumber</span></span>|<span data-ttu-id="b699b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b699b-112">Int32</span></span>|<span data-ttu-id="b699b-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="b699b-113">Lower number.</span></span>|
|<span data-ttu-id="b699b-114">Уппернумбер</span><span class="sxs-lookup"><span data-stu-id="b699b-114">upperNumber</span></span>|<span data-ttu-id="b699b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b699b-115">Int32</span></span>|<span data-ttu-id="b699b-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="b699b-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b699b-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="b699b-117">Relationships</span></span>
<span data-ttu-id="b699b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b699b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b699b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b699b-119">JSON Representation</span></span>
<span data-ttu-id="b699b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b699b-120">Here is a JSON representation of the resource.</span></span>
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





