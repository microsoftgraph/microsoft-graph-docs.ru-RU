---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643764"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="ad22d-104">Тип ресурса networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="ad22d-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="ad22d-105">Указывает сведения, связанные с сетевую папку.</span><span class="sxs-lookup"><span data-stu-id="ad22d-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="ad22d-106">.</span><span class="sxs-lookup"><span data-stu-id="ad22d-106"></span></span>



## <a name="properties"></a><span data-ttu-id="ad22d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad22d-107">Properties</span></span>
| <span data-ttu-id="ad22d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad22d-108">Property</span></span>     | <span data-ttu-id="ad22d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ad22d-109">Type</span></span>   |<span data-ttu-id="ad22d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad22d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad22d-111">networkType</span><span class="sxs-lookup"><span data-stu-id="ad22d-111">networkType</span></span>|<span data-ttu-id="ad22d-112">String</span><span class="sxs-lookup"><span data-stu-id="ad22d-112">String</span></span>|<span data-ttu-id="ad22d-113">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="ad22d-113">Provides the type of the network.</span></span> <span data-ttu-id="ad22d-114">Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.</span><span class="sxs-lookup"><span data-stu-id="ad22d-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="ad22d-115">networkName</span><span class="sxs-lookup"><span data-stu-id="ad22d-115">networkName</span></span>|<span data-ttu-id="ad22d-116">String</span><span class="sxs-lookup"><span data-stu-id="ad22d-116">String</span></span>|<span data-ttu-id="ad22d-117">Имя сети.</span><span class="sxs-lookup"><span data-stu-id="ad22d-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ad22d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad22d-118">JSON representation</span></span>

<span data-ttu-id="ad22d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad22d-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
