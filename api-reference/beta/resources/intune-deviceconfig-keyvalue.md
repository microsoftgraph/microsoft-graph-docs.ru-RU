---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 592f3ff070ab7440d5c16d5380b556993915e6ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946127"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="08cea-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="08cea-103">keyValue resource type</span></span>

> <span data-ttu-id="08cea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08cea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08cea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08cea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08cea-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="08cea-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="08cea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08cea-107">Properties</span></span>
|<span data-ttu-id="08cea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08cea-108">Property</span></span>|<span data-ttu-id="08cea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08cea-109">Type</span></span>|<span data-ttu-id="08cea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08cea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08cea-111">ключа</span><span class="sxs-lookup"><span data-stu-id="08cea-111">key</span></span>|<span data-ttu-id="08cea-112">Строка</span><span class="sxs-lookup"><span data-stu-id="08cea-112">String</span></span>|<span data-ttu-id="08cea-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="08cea-113">Key.</span></span>|
|<span data-ttu-id="08cea-114">value</span><span class="sxs-lookup"><span data-stu-id="08cea-114">value</span></span>|<span data-ttu-id="08cea-115">String</span><span class="sxs-lookup"><span data-stu-id="08cea-115">String</span></span>|<span data-ttu-id="08cea-116">Значение</span><span class="sxs-lookup"><span data-stu-id="08cea-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08cea-117">Связи</span><span class="sxs-lookup"><span data-stu-id="08cea-117">Relationships</span></span>
<span data-ttu-id="08cea-118">Нет</span><span class="sxs-lookup"><span data-stu-id="08cea-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08cea-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08cea-119">JSON Representation</span></span>
<span data-ttu-id="08cea-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08cea-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




