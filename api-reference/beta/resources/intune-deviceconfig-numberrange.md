---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8912b6a0cba8c1265060a53a8f32d9455b3bba39
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951033"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="db351-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="db351-103">numberRange resource type</span></span>

> <span data-ttu-id="db351-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db351-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db351-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db351-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db351-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="db351-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="db351-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db351-107">Properties</span></span>
|<span data-ttu-id="db351-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db351-108">Property</span></span>|<span data-ttu-id="db351-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db351-109">Type</span></span>|<span data-ttu-id="db351-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db351-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db351-111">Ловернумбер</span><span class="sxs-lookup"><span data-stu-id="db351-111">lowerNumber</span></span>|<span data-ttu-id="db351-112">Int32</span><span class="sxs-lookup"><span data-stu-id="db351-112">Int32</span></span>|<span data-ttu-id="db351-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="db351-113">Lower number.</span></span>|
|<span data-ttu-id="db351-114">Уппернумбер</span><span class="sxs-lookup"><span data-stu-id="db351-114">upperNumber</span></span>|<span data-ttu-id="db351-115">Int32</span><span class="sxs-lookup"><span data-stu-id="db351-115">Int32</span></span>|<span data-ttu-id="db351-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="db351-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db351-117">Связи</span><span class="sxs-lookup"><span data-stu-id="db351-117">Relationships</span></span>
<span data-ttu-id="db351-118">Нет</span><span class="sxs-lookup"><span data-stu-id="db351-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db351-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db351-119">JSON Representation</span></span>
<span data-ttu-id="db351-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db351-120">Here is a JSON representation of the resource.</span></span>
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




