---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258739"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="2a336-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="2a336-103">keyValuePair resource type</span></span>

> <span data-ttu-id="2a336-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a336-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a336-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="2a336-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="2a336-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a336-106">Properties</span></span>
|<span data-ttu-id="2a336-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a336-107">Property</span></span>|<span data-ttu-id="2a336-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2a336-108">Type</span></span>|<span data-ttu-id="2a336-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a336-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a336-110">name</span><span class="sxs-lookup"><span data-stu-id="2a336-110">name</span></span>|<span data-ttu-id="2a336-111">String</span><span class="sxs-lookup"><span data-stu-id="2a336-111">String</span></span>|<span data-ttu-id="2a336-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="2a336-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="2a336-113">value</span><span class="sxs-lookup"><span data-stu-id="2a336-113">value</span></span>|<span data-ttu-id="2a336-114">String</span><span class="sxs-lookup"><span data-stu-id="2a336-114">String</span></span>|<span data-ttu-id="2a336-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="2a336-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a336-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2a336-116">Relationships</span></span>
<span data-ttu-id="2a336-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2a336-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a336-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a336-118">JSON Representation</span></span>
<span data-ttu-id="2a336-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a336-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



