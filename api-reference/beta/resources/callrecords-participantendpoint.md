---
title: Тип ресурса ПартиЦипантендпоинт
description: Тип ПартиЦипантендпоинт
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed7e27629bb63c23f88cc71410470d1d6aac3714
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601687"
---
# <a name="participantendpoint-resource-type"></a><span data-ttu-id="78caa-103">Тип ресурса ПартиЦипантендпоинт</span><span class="sxs-lookup"><span data-stu-id="78caa-103">participantEndpoint resource type</span></span>

<span data-ttu-id="78caa-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="78caa-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78caa-105">Представляет конечную точку участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="78caa-105">Represents an participant endpoint in a call.</span></span> <span data-ttu-id="78caa-106">Конечная точка представляет пользователя или подобную пользователю сущность.</span><span class="sxs-lookup"><span data-stu-id="78caa-106">The endpoint represents a user or user-like entity.</span></span> <span data-ttu-id="78caa-107">Наследуется от типа [конечной точки](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="78caa-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="78caa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78caa-108">Properties</span></span>

| <span data-ttu-id="78caa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78caa-109">Property</span></span>     | <span data-ttu-id="78caa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78caa-110">Type</span></span>        | <span data-ttu-id="78caa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78caa-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78caa-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="78caa-112">userAgent</span></span>|[<span data-ttu-id="78caa-113">Microsoft. Graph. Каллрекордс. userAgent</span><span class="sxs-lookup"><span data-stu-id="78caa-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="78caa-114">Пользователь — агент, указанный этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="78caa-114">User-agent reported by this endpoint.</span></span>|
|<span data-ttu-id="78caa-115">feedback</span><span class="sxs-lookup"><span data-stu-id="78caa-115">feedback</span></span>|[<span data-ttu-id="78caa-116">Microsoft. Graph. Каллрекордс. Усерфидбакк</span><span class="sxs-lookup"><span data-stu-id="78caa-116">microsoft.graph.callRecords.userFeedback</span></span>](callrecords-userfeedback.md)|<span data-ttu-id="78caa-117">Обратная связь, предоставленная пользователем данной конечной точки относительно качества сеанса.</span><span class="sxs-lookup"><span data-stu-id="78caa-117">The feedback provided by the user of this endpoint about the quality of the session.</span></span>|
|<span data-ttu-id="78caa-118">хищения</span><span class="sxs-lookup"><span data-stu-id="78caa-118">identity</span></span>|[<span data-ttu-id="78caa-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="78caa-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="78caa-120">Удостоверение, связанное с конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="78caa-120">Identity associated with the endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78caa-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78caa-121">JSON representation</span></span>

<span data-ttu-id="78caa-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78caa-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

