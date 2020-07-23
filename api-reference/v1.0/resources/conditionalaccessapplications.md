---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b09a3531d3734aed67e9ff91fee1d917f76054b
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384687"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="3ab9c-103">Тип ресурса Кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="3ab9c-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="3ab9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ab9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ab9c-105">Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="3ab9c-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3ab9c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ab9c-106">Properties</span></span>

| <span data-ttu-id="3ab9c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ab9c-107">Property</span></span>     | <span data-ttu-id="3ab9c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3ab9c-108">Type</span></span>        | <span data-ttu-id="3ab9c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ab9c-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3ab9c-110">инклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="3ab9c-110">includeApplications</span></span> | <span data-ttu-id="3ab9c-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ab9c-111">String collection</span></span> | <span data-ttu-id="3ab9c-112">Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс).</span><span class="sxs-lookup"><span data-stu-id="3ab9c-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="3ab9c-113">Также можно задать значение `All` .</span><span class="sxs-lookup"><span data-stu-id="3ab9c-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="3ab9c-114">ексклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="3ab9c-114">excludeApplications</span></span> | <span data-ttu-id="3ab9c-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ab9c-115">String collection</span></span> | <span data-ttu-id="3ab9c-116">Список идентификаторов приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="3ab9c-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="3ab9c-117">инклудеусерактионс</span><span class="sxs-lookup"><span data-stu-id="3ab9c-117">includeUserActions</span></span> | <span data-ttu-id="3ab9c-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ab9c-118">String collection</span></span> | <span data-ttu-id="3ab9c-119">Включаемые действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ab9c-119">User actions to include.</span></span> <span data-ttu-id="3ab9c-120">Пример: `urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="3ab9c-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="3ab9c-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3ab9c-121">Relationships</span></span>

<span data-ttu-id="3ab9c-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ab9c-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ab9c-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ab9c-123">JSON representation</span></span>

<span data-ttu-id="3ab9c-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ab9c-124">The following is a JSON representation of the resource.</span></span>

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
