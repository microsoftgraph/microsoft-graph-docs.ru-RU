---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd9c57961bee93e7d01e504bccb8671a8f1dd449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522034"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="e9831-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="e9831-103">participantInfo resource type</span></span>

<span data-ttu-id="e9831-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e9831-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9831-105">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="e9831-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="e9831-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9831-106">Properties</span></span>

| <span data-ttu-id="e9831-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9831-107">Property</span></span>       | <span data-ttu-id="e9831-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9831-108">Type</span></span>                          | <span data-ttu-id="e9831-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9831-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e9831-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="e9831-110">countryCode</span></span>    | <span data-ttu-id="e9831-111">String</span><span class="sxs-lookup"><span data-stu-id="e9831-111">String</span></span>                        | <span data-ttu-id="e9831-112">Код страны ISO 3166-1 Alpha-2 в наиболее подсчитанном физическом расположении участника в начале звонка.</span><span class="sxs-lookup"><span data-stu-id="e9831-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="e9831-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9831-113">Read-only.</span></span>                             |
| <span data-ttu-id="e9831-114">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="e9831-114">endpointType</span></span>   | <span data-ttu-id="e9831-115">String</span><span class="sxs-lookup"><span data-stu-id="e9831-115">String</span></span>                        | <span data-ttu-id="e9831-116">Тип конечной точки, используемой участником.</span><span class="sxs-lookup"><span data-stu-id="e9831-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="e9831-117">Возможные значения: `default`, `skypeForBusiness`, или. `skypeForBusinessVoipPhone`</span><span class="sxs-lookup"><span data-stu-id="e9831-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="e9831-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9831-118">Read-only.</span></span>              |
| <span data-ttu-id="e9831-119">хищения</span><span class="sxs-lookup"><span data-stu-id="e9831-119">identity</span></span>       | [<span data-ttu-id="e9831-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9831-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="e9831-121">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="e9831-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="e9831-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9831-122">Read-only.</span></span>                                                                             |
| <span data-ttu-id="e9831-123">languageId</span><span class="sxs-lookup"><span data-stu-id="e9831-123">languageId</span></span>     | <span data-ttu-id="e9831-124">String</span><span class="sxs-lookup"><span data-stu-id="e9831-124">String</span></span>                        | <span data-ttu-id="e9831-125">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="e9831-125">The language culture string.</span></span> <span data-ttu-id="e9831-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9831-126">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="e9831-127">региональных</span><span class="sxs-lookup"><span data-stu-id="e9831-127">region</span></span>         | <span data-ttu-id="e9831-128">String</span><span class="sxs-lookup"><span data-stu-id="e9831-128">String</span></span>                        | <span data-ttu-id="e9831-129">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="e9831-129">The home region of the participant.</span></span> <span data-ttu-id="e9831-130">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="e9831-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="e9831-131">Это не изменяется в зависимости от текущего физического расположения участника, в отличие от countryCode.</span><span class="sxs-lookup"><span data-stu-id="e9831-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="e9831-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9831-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9831-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9831-133">JSON representation</span></span>

<span data-ttu-id="e9831-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9831-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
