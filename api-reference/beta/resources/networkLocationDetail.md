---
title: Тип ресурса Нетворклокатиондетаил
description: Предоставляет имя и тип сети, из которой пользователь выполнил вход.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8cbf60f7e7e370c5813623643f9d14cb324950cc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939511"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="c0a19-103">Тип ресурса Нетворклокатиондетаил</span><span class="sxs-lookup"><span data-stu-id="c0a19-103">networkLocationDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0a19-104">Предоставляет имя и тип сети, из которой пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="c0a19-104">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="c0a19-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0a19-105">Properties</span></span>

| <span data-ttu-id="c0a19-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0a19-106">Property</span></span>     | <span data-ttu-id="c0a19-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a19-107">Type</span></span>        | <span data-ttu-id="c0a19-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a19-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0a19-109">нетворкнамес</span><span class="sxs-lookup"><span data-stu-id="c0a19-109">networkNames</span></span>|<span data-ttu-id="c0a19-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c0a19-110">String collection</span></span>|<span data-ttu-id="c0a19-111">Предоставляет имя сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="c0a19-111">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="c0a19-112">нетворктипе</span><span class="sxs-lookup"><span data-stu-id="c0a19-112">networkType</span></span>|<span data-ttu-id="c0a19-113">нетворктипе</span><span class="sxs-lookup"><span data-stu-id="c0a19-113">networkType</span></span>| <span data-ttu-id="c0a19-114">Предоставляет тип сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="c0a19-114">Provides the type of network used when signing in.</span></span> <span data-ttu-id="c0a19-115">Возможные значения: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c0a19-115">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0a19-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0a19-116">JSON representation</span></span>

<span data-ttu-id="c0a19-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0a19-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->