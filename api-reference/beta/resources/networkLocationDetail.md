---
title: Тип ресурса Нетворклокатиондетаил
description: Показывает сведения, связанные с сетевым расположением. .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342179"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="1f395-104">Тип ресурса Нетворклокатиондетаил</span><span class="sxs-lookup"><span data-stu-id="1f395-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="1f395-105">Показывает сведения, связанные с сетевым расположением.</span><span class="sxs-lookup"><span data-stu-id="1f395-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="1f395-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f395-106">Properties</span></span>
| <span data-ttu-id="1f395-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f395-107">Property</span></span>     | <span data-ttu-id="1f395-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1f395-108">Type</span></span>   |<span data-ttu-id="1f395-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1f395-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f395-110">Нетворктипе</span><span class="sxs-lookup"><span data-stu-id="1f395-110">networkType</span></span>|<span data-ttu-id="1f395-111">Нетворктипе</span><span class="sxs-lookup"><span data-stu-id="1f395-111">networkType</span></span>|<span data-ttu-id="1f395-112">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="1f395-112">Provides the type of the network.</span></span> <span data-ttu-id="1f395-113">`intranet`Возможные значения: `extranet`, `namedNetwork`, и. `trusted`</span><span class="sxs-lookup"><span data-stu-id="1f395-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="1f395-114">Нетворкнамес</span><span class="sxs-lookup"><span data-stu-id="1f395-114">networkNames</span></span>|<span data-ttu-id="1f395-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f395-115">String collection</span></span>|<span data-ttu-id="1f395-116">Имена сетей.</span><span class="sxs-lookup"><span data-stu-id="1f395-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1f395-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f395-117">JSON representation</span></span>

<span data-ttu-id="1f395-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f395-118">Here is a JSON representation of the resource.</span></span>

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
