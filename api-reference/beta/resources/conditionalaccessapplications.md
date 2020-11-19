---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba904fec35830bef6cc5a74daa1c4938bd99d250
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269912"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="52dd6-103">Тип ресурса Кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="52dd6-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="52dd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52dd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52dd6-105">Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="52dd6-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="52dd6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="52dd6-106">Properties</span></span>

| <span data-ttu-id="52dd6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="52dd6-107">Property</span></span> | <span data-ttu-id="52dd6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="52dd6-108">Type</span></span> | <span data-ttu-id="52dd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="52dd6-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="52dd6-110">инклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="52dd6-110">includeApplications</span></span> | <span data-ttu-id="52dd6-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52dd6-111">String collection</span></span> | <span data-ttu-id="52dd6-112">Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс).</span><span class="sxs-lookup"><span data-stu-id="52dd6-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="52dd6-113">Также можно задать значение `All` .</span><span class="sxs-lookup"><span data-stu-id="52dd6-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="52dd6-114">ексклудеаппликатионс</span><span class="sxs-lookup"><span data-stu-id="52dd6-114">excludeApplications</span></span> | <span data-ttu-id="52dd6-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52dd6-115">String collection</span></span> | <span data-ttu-id="52dd6-116">Список идентификаторов приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="52dd6-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="52dd6-117">инклудеусерактионс</span><span class="sxs-lookup"><span data-stu-id="52dd6-117">includeUserActions</span></span> | <span data-ttu-id="52dd6-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52dd6-118">String collection</span></span> | <span data-ttu-id="52dd6-119">Включаемые действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="52dd6-119">User actions to include.</span></span> <span data-ttu-id="52dd6-120">Поддерживаемые значения: `urn:user:registersecurityinfo` и `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="52dd6-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="52dd6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="52dd6-121">Relationships</span></span>

<span data-ttu-id="52dd6-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="52dd6-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52dd6-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="52dd6-123">JSON representation</span></span>

<span data-ttu-id="52dd6-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52dd6-124">The following is a JSON representation of the resource.</span></span>

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

