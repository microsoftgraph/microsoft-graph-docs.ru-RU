---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a29fcb627a1777b2fc0a4863bbab27d5fa364982
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325521"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="f5777-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="f5777-103">keyValue resource type</span></span>

> <span data-ttu-id="f5777-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5777-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5777-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5777-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5777-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="f5777-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f5777-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5777-107">Properties</span></span>
|<span data-ttu-id="f5777-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5777-108">Property</span></span>|<span data-ttu-id="f5777-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f5777-109">Type</span></span>|<span data-ttu-id="f5777-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5777-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5777-111">ключа</span><span class="sxs-lookup"><span data-stu-id="f5777-111">key</span></span>|<span data-ttu-id="f5777-112">String</span><span class="sxs-lookup"><span data-stu-id="f5777-112">String</span></span>|<span data-ttu-id="f5777-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="f5777-113">Key.</span></span>|
|<span data-ttu-id="f5777-114">value</span><span class="sxs-lookup"><span data-stu-id="f5777-114">value</span></span>|<span data-ttu-id="f5777-115">String</span><span class="sxs-lookup"><span data-stu-id="f5777-115">String</span></span>|<span data-ttu-id="f5777-116">Значение</span><span class="sxs-lookup"><span data-stu-id="f5777-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5777-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f5777-117">Relationships</span></span>
<span data-ttu-id="f5777-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f5777-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5777-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5777-119">JSON Representation</span></span>
<span data-ttu-id="f5777-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5777-120">Here is a JSON representation of the resource.</span></span>
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



