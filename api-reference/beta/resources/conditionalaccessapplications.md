---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163d8f958a400c9c478b0aca865bdfa077c8d60
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638591"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="c72e9-103">Тип ресурса Кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="c72e9-103">conditionalAccessApplications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c72e9-104">Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="c72e9-104">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="c72e9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c72e9-105">Properties</span></span>

| <span data-ttu-id="c72e9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c72e9-106">Property</span></span> | <span data-ttu-id="c72e9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c72e9-107">Type</span></span> | <span data-ttu-id="c72e9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c72e9-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c72e9-109">инклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="c72e9-109">includeApplications</span></span> | <span data-ttu-id="c72e9-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c72e9-110">String collection</span></span> | <span data-ttu-id="c72e9-111">Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс).</span><span class="sxs-lookup"><span data-stu-id="c72e9-111">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="c72e9-112">Также можно задать значение `All`.</span><span class="sxs-lookup"><span data-stu-id="c72e9-112">Can also be set to `All`.</span></span> |
| <span data-ttu-id="c72e9-113">ексклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="c72e9-113">excludeApplications</span></span> | <span data-ttu-id="c72e9-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c72e9-114">String collection</span></span> | <span data-ttu-id="c72e9-115">Список идентификаторов приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="c72e9-115">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="c72e9-116">инклудеусерактионс</span><span class="sxs-lookup"><span data-stu-id="c72e9-116">includeUserActions</span></span> | <span data-ttu-id="c72e9-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c72e9-117">String collection</span></span> | <span data-ttu-id="c72e9-118">Включаемые действия пользователя (например, `urn:user:registersecurityinfo`);</span><span class="sxs-lookup"><span data-stu-id="c72e9-118">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="c72e9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c72e9-119">Relationships</span></span>

<span data-ttu-id="c72e9-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c72e9-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c72e9-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c72e9-121">JSON representation</span></span>

<span data-ttu-id="c72e9-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c72e9-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->