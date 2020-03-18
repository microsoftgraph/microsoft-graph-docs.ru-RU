---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e875ba06ff704f01cc2fd7b7dd48c2b8cfcfba63
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790386"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="a5078-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="a5078-103">keyValue resource type</span></span>

> <span data-ttu-id="a5078-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5078-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5078-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5078-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5078-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="a5078-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a5078-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5078-107">Properties</span></span>
|<span data-ttu-id="a5078-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5078-108">Property</span></span>|<span data-ttu-id="a5078-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5078-109">Type</span></span>|<span data-ttu-id="a5078-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5078-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5078-111">ключа</span><span class="sxs-lookup"><span data-stu-id="a5078-111">key</span></span>|<span data-ttu-id="a5078-112">String</span><span class="sxs-lookup"><span data-stu-id="a5078-112">String</span></span>|<span data-ttu-id="a5078-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="a5078-113">Key.</span></span>|
|<span data-ttu-id="a5078-114">value</span><span class="sxs-lookup"><span data-stu-id="a5078-114">value</span></span>|<span data-ttu-id="a5078-115">String</span><span class="sxs-lookup"><span data-stu-id="a5078-115">String</span></span>|<span data-ttu-id="a5078-116">Значение</span><span class="sxs-lookup"><span data-stu-id="a5078-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5078-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a5078-117">Relationships</span></span>
<span data-ttu-id="a5078-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a5078-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5078-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5078-119">JSON Representation</span></span>
<span data-ttu-id="a5078-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5078-120">Here is a JSON representation of the resource.</span></span>
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



