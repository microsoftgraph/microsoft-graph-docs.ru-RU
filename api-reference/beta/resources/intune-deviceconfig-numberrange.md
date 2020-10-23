---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f637cb10e36ba1f2d7c45e391adc64c6e9eb00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723001"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="893c7-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="893c7-103">numberRange resource type</span></span>

<span data-ttu-id="893c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="893c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="893c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="893c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="893c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="893c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="893c7-107">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="893c7-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="893c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="893c7-108">Properties</span></span>
|<span data-ttu-id="893c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="893c7-109">Property</span></span>|<span data-ttu-id="893c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="893c7-110">Type</span></span>|<span data-ttu-id="893c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="893c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893c7-112">ловернумбер</span><span class="sxs-lookup"><span data-stu-id="893c7-112">lowerNumber</span></span>|<span data-ttu-id="893c7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="893c7-113">Int32</span></span>|<span data-ttu-id="893c7-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="893c7-114">Lower number.</span></span>|
|<span data-ttu-id="893c7-115">уппернумбер</span><span class="sxs-lookup"><span data-stu-id="893c7-115">upperNumber</span></span>|<span data-ttu-id="893c7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="893c7-116">Int32</span></span>|<span data-ttu-id="893c7-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="893c7-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="893c7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="893c7-118">Relationships</span></span>
<span data-ttu-id="893c7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="893c7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="893c7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="893c7-120">JSON Representation</span></span>
<span data-ttu-id="893c7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="893c7-121">Here is a JSON representation of the resource.</span></span>
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





