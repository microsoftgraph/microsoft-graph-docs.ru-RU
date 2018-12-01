---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079295"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="f3644-104">Тип ресурса networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="f3644-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="f3644-105">Указывает сведения, связанные с сетевую папку.</span><span class="sxs-lookup"><span data-stu-id="f3644-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="f3644-106">.</span><span class="sxs-lookup"><span data-stu-id="f3644-106"></span></span>



## <a name="properties"></a><span data-ttu-id="f3644-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3644-107">Properties</span></span>
| <span data-ttu-id="f3644-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3644-108">Property</span></span>     | <span data-ttu-id="f3644-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3644-109">Type</span></span>   |<span data-ttu-id="f3644-110">Description</span><span class="sxs-lookup"><span data-stu-id="f3644-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3644-111">networkType</span><span class="sxs-lookup"><span data-stu-id="f3644-111">networkType</span></span>|<span data-ttu-id="f3644-112">String</span><span class="sxs-lookup"><span data-stu-id="f3644-112">String</span></span>|<span data-ttu-id="f3644-113">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="f3644-113">Provides the type of the network.</span></span> <span data-ttu-id="f3644-114">Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.</span><span class="sxs-lookup"><span data-stu-id="f3644-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="f3644-115">networkName</span><span class="sxs-lookup"><span data-stu-id="f3644-115">networkName</span></span>|<span data-ttu-id="f3644-116">String</span><span class="sxs-lookup"><span data-stu-id="f3644-116">String</span></span>|<span data-ttu-id="f3644-117">Имя сети.</span><span class="sxs-lookup"><span data-stu-id="f3644-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f3644-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3644-118">JSON representation</span></span>

<span data-ttu-id="f3644-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3644-119">Here is a JSON representation of the resource.</span></span>

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