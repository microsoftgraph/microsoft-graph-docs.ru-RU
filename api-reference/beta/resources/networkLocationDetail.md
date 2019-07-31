---
title: Тип ресурса Нетворклокатиондетаил
description: Показывает сведения, связанные с сетевым расположением. .
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b7e12a87889909737cac9a52fadf64231f7f2a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009610"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="b9daa-104">Тип ресурса Нетворклокатиондетаил</span><span class="sxs-lookup"><span data-stu-id="b9daa-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="b9daa-105">Показывает сведения, связанные с сетевым расположением.</span><span class="sxs-lookup"><span data-stu-id="b9daa-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="b9daa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9daa-106">Properties</span></span>
| <span data-ttu-id="b9daa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9daa-107">Property</span></span>     | <span data-ttu-id="b9daa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b9daa-108">Type</span></span>   |<span data-ttu-id="b9daa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b9daa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9daa-110">Нетворктипе</span><span class="sxs-lookup"><span data-stu-id="b9daa-110">networkType</span></span>|<span data-ttu-id="b9daa-111">Нетворктипе</span><span class="sxs-lookup"><span data-stu-id="b9daa-111">networkType</span></span>|<span data-ttu-id="b9daa-112">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="b9daa-112">Provides the type of the network.</span></span> <span data-ttu-id="b9daa-113">`intranet`Возможные значения: `extranet`, `namedNetwork`, и. `trusted`</span><span class="sxs-lookup"><span data-stu-id="b9daa-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="b9daa-114">Нетворкнамес</span><span class="sxs-lookup"><span data-stu-id="b9daa-114">networkNames</span></span>|<span data-ttu-id="b9daa-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b9daa-115">String collection</span></span>|<span data-ttu-id="b9daa-116">Имена сетей.</span><span class="sxs-lookup"><span data-stu-id="b9daa-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b9daa-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9daa-117">JSON representation</span></span>

<span data-ttu-id="b9daa-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9daa-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
