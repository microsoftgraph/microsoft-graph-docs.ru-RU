---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 998df44aaad34bad21ef23d8134465b74cd71ca7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001014"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="515f2-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="515f2-103">keyValue resource type</span></span>

> <span data-ttu-id="515f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="515f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="515f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="515f2-106">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="515f2-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="515f2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="515f2-107">Properties</span></span>
|<span data-ttu-id="515f2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="515f2-108">Property</span></span>|<span data-ttu-id="515f2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="515f2-109">Type</span></span>|<span data-ttu-id="515f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="515f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="515f2-111">ключа</span><span class="sxs-lookup"><span data-stu-id="515f2-111">key</span></span>|<span data-ttu-id="515f2-112">String</span><span class="sxs-lookup"><span data-stu-id="515f2-112">String</span></span>|<span data-ttu-id="515f2-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="515f2-113">Key.</span></span>|
|<span data-ttu-id="515f2-114">value</span><span class="sxs-lookup"><span data-stu-id="515f2-114">value</span></span>|<span data-ttu-id="515f2-115">String</span><span class="sxs-lookup"><span data-stu-id="515f2-115">String</span></span>|<span data-ttu-id="515f2-116">Значение</span><span class="sxs-lookup"><span data-stu-id="515f2-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="515f2-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="515f2-117">Relationships</span></span>
<span data-ttu-id="515f2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="515f2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="515f2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="515f2-119">JSON Representation</span></span>
<span data-ttu-id="515f2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="515f2-120">Here is a JSON representation of the resource.</span></span>
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





