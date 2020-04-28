---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1ce31fd39c94299ccb6e2a0cc1330a44a149db3
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916853"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="4e5f7-103">Тип ресурса Кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="4e5f7-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="4e5f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e5f7-105">Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="4e5f7-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="4e5f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e5f7-106">Properties</span></span>

| <span data-ttu-id="4e5f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e5f7-107">Property</span></span> | <span data-ttu-id="4e5f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5f7-108">Type</span></span> | <span data-ttu-id="4e5f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5f7-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="4e5f7-110">инклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="4e5f7-110">includeApplications</span></span> | <span data-ttu-id="4e5f7-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4e5f7-111">String collection</span></span> | <span data-ttu-id="4e5f7-112">Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс).</span><span class="sxs-lookup"><span data-stu-id="4e5f7-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="4e5f7-113">Также можно задать значение `All`.</span><span class="sxs-lookup"><span data-stu-id="4e5f7-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="4e5f7-114">ексклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="4e5f7-114">excludeApplications</span></span> | <span data-ttu-id="4e5f7-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4e5f7-115">String collection</span></span> | <span data-ttu-id="4e5f7-116">Список идентификаторов приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="4e5f7-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="4e5f7-117">инклудеусерактионс</span><span class="sxs-lookup"><span data-stu-id="4e5f7-117">includeUserActions</span></span> | <span data-ttu-id="4e5f7-118">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4e5f7-118">String collection</span></span> | <span data-ttu-id="4e5f7-119">Включаемые действия пользователя (например, `urn:user:registersecurityinfo`);</span><span class="sxs-lookup"><span data-stu-id="4e5f7-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="4e5f7-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4e5f7-120">Relationships</span></span>

<span data-ttu-id="4e5f7-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e5f7-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e5f7-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e5f7-122">JSON representation</span></span>

<span data-ttu-id="4e5f7-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5f7-123">The following is a JSON representation of the resource.</span></span>

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