---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834323"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="a348c-104">Тип ресурса networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="a348c-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="a348c-105">Указывает сведения, связанные с сетевую папку.</span><span class="sxs-lookup"><span data-stu-id="a348c-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="a348c-106">.</span><span class="sxs-lookup"><span data-stu-id="a348c-106"></span></span>



## <a name="properties"></a><span data-ttu-id="a348c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a348c-107">Properties</span></span>
| <span data-ttu-id="a348c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a348c-108">Property</span></span>     | <span data-ttu-id="a348c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a348c-109">Type</span></span>   |<span data-ttu-id="a348c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a348c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a348c-111">networkType</span><span class="sxs-lookup"><span data-stu-id="a348c-111">networkType</span></span>|<span data-ttu-id="a348c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a348c-112">String</span></span>|<span data-ttu-id="a348c-113">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="a348c-113">Provides the type of the network.</span></span> <span data-ttu-id="a348c-114">Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.</span><span class="sxs-lookup"><span data-stu-id="a348c-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="a348c-115">networkName</span><span class="sxs-lookup"><span data-stu-id="a348c-115">networkName</span></span>|<span data-ttu-id="a348c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a348c-116">String</span></span>|<span data-ttu-id="a348c-117">Имя сети.</span><span class="sxs-lookup"><span data-stu-id="a348c-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a348c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a348c-118">JSON representation</span></span>

<span data-ttu-id="a348c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a348c-119">Here is a JSON representation of the resource.</span></span>

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
