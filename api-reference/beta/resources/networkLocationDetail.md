---
title: Тип ресурса networkLocationDetail
description: Указывает сведения, связанные с сетевую папку. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570941"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="f0a15-104">Тип ресурса networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="f0a15-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="f0a15-105">Указывает сведения, связанные с сетевую папку.</span><span class="sxs-lookup"><span data-stu-id="f0a15-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="f0a15-106">.</span><span class="sxs-lookup"><span data-stu-id="f0a15-106"></span></span>



## <a name="properties"></a><span data-ttu-id="f0a15-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0a15-107">Properties</span></span>
| <span data-ttu-id="f0a15-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0a15-108">Property</span></span>     | <span data-ttu-id="f0a15-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0a15-109">Type</span></span>   |<span data-ttu-id="f0a15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0a15-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a15-111">networkType</span><span class="sxs-lookup"><span data-stu-id="f0a15-111">networkType</span></span>| <span data-ttu-id="f0a15-112">Строка перечисления</span><span class="sxs-lookup"><span data-stu-id="f0a15-112">enum-string</span></span> |<span data-ttu-id="f0a15-113">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="f0a15-113">Provides the type of the network.</span></span> <span data-ttu-id="f0a15-114">Возможные значения: `intranet`, `extranet`, `namedNetwork`, и `trusted`.</span><span class="sxs-lookup"><span data-stu-id="f0a15-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="f0a15-115">networkName</span><span class="sxs-lookup"><span data-stu-id="f0a15-115">networkName</span></span>|<span data-ttu-id="f0a15-116">Строка</span><span class="sxs-lookup"><span data-stu-id="f0a15-116">String</span></span>|<span data-ttu-id="f0a15-117">Имя сети.</span><span class="sxs-lookup"><span data-stu-id="f0a15-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f0a15-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0a15-118">JSON representation</span></span>

<span data-ttu-id="f0a15-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0a15-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
