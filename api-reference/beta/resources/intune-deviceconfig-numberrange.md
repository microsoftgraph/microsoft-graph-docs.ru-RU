---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e3073de15fc84f5a8cb755d6aad32caaf1ee29f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788494"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="4b943-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="4b943-103">numberRange resource type</span></span>

> <span data-ttu-id="4b943-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b943-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b943-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b943-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b943-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="4b943-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="4b943-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b943-107">Properties</span></span>
|<span data-ttu-id="4b943-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b943-108">Property</span></span>|<span data-ttu-id="4b943-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b943-109">Type</span></span>|<span data-ttu-id="4b943-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b943-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b943-111">ловернумбер</span><span class="sxs-lookup"><span data-stu-id="4b943-111">lowerNumber</span></span>|<span data-ttu-id="4b943-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4b943-112">Int32</span></span>|<span data-ttu-id="4b943-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="4b943-113">Lower number.</span></span>|
|<span data-ttu-id="4b943-114">уппернумбер</span><span class="sxs-lookup"><span data-stu-id="4b943-114">upperNumber</span></span>|<span data-ttu-id="4b943-115">Int32</span><span class="sxs-lookup"><span data-stu-id="4b943-115">Int32</span></span>|<span data-ttu-id="4b943-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="4b943-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b943-117">Связи</span><span class="sxs-lookup"><span data-stu-id="4b943-117">Relationships</span></span>
<span data-ttu-id="4b943-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4b943-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b943-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b943-119">JSON Representation</span></span>
<span data-ttu-id="4b943-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b943-120">Here is a JSON representation of the resource.</span></span>
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



