---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597f6d2101e4549336693f1cff7ce64199b46287
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155498"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="3307c-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="3307c-103">keyValue resource type</span></span>

> <span data-ttu-id="3307c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3307c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3307c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3307c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3307c-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="3307c-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3307c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3307c-107">Properties</span></span>
|<span data-ttu-id="3307c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3307c-108">Property</span></span>|<span data-ttu-id="3307c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3307c-109">Type</span></span>|<span data-ttu-id="3307c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3307c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3307c-111">key</span><span class="sxs-lookup"><span data-stu-id="3307c-111">key</span></span>|<span data-ttu-id="3307c-112">String</span><span class="sxs-lookup"><span data-stu-id="3307c-112">String</span></span>|<span data-ttu-id="3307c-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="3307c-113">Key.</span></span>|
|<span data-ttu-id="3307c-114">value</span><span class="sxs-lookup"><span data-stu-id="3307c-114">value</span></span>|<span data-ttu-id="3307c-115">String</span><span class="sxs-lookup"><span data-stu-id="3307c-115">String</span></span>|<span data-ttu-id="3307c-116">Значение</span><span class="sxs-lookup"><span data-stu-id="3307c-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3307c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="3307c-117">Relationships</span></span>
<span data-ttu-id="3307c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3307c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3307c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3307c-119">JSON Representation</span></span>
<span data-ttu-id="3307c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3307c-120">Here is a JSON representation of the resource.</span></span>
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




