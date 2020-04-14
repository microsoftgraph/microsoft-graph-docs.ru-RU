---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6484ec54b5e39ad2e6b189cc70c05fd666b81297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413526"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="bf555-103">Тип ресурса Кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="bf555-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="bf555-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf555-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf555-105">Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="bf555-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="bf555-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf555-106">Properties</span></span>

| <span data-ttu-id="bf555-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf555-107">Property</span></span> | <span data-ttu-id="bf555-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bf555-108">Type</span></span> | <span data-ttu-id="bf555-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bf555-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="bf555-110">инклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="bf555-110">includeApplications</span></span> | <span data-ttu-id="bf555-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf555-111">String collection</span></span> | <span data-ttu-id="bf555-112">Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс).</span><span class="sxs-lookup"><span data-stu-id="bf555-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="bf555-113">Также можно задать значение `All`.</span><span class="sxs-lookup"><span data-stu-id="bf555-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="bf555-114">ексклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="bf555-114">excludeApplications</span></span> | <span data-ttu-id="bf555-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf555-115">String collection</span></span> | <span data-ttu-id="bf555-116">Список идентификаторов приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="bf555-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="bf555-117">инклудеусерактионс</span><span class="sxs-lookup"><span data-stu-id="bf555-117">includeUserActions</span></span> | <span data-ttu-id="bf555-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf555-118">String collection</span></span> | <span data-ttu-id="bf555-119">Включаемые действия пользователя (например, `urn:user:registersecurityinfo`);</span><span class="sxs-lookup"><span data-stu-id="bf555-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="bf555-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bf555-120">Relationships</span></span>

<span data-ttu-id="bf555-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf555-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf555-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bf555-122">JSON representation</span></span>

<span data-ttu-id="bf555-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf555-123">The following is a JSON representation of the resource.</span></span>

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