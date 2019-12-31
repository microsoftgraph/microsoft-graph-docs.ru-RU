---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b3d8671c33a0040fde8671a2d97b67dae0e94b28
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913585"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="0846a-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="0846a-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0846a-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="0846a-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="0846a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0846a-105">Properties</span></span>

| <span data-ttu-id="0846a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0846a-106">Property</span></span>       | <span data-ttu-id="0846a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0846a-107">Type</span></span>                          | <span data-ttu-id="0846a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0846a-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0846a-109">countryCode</span><span class="sxs-lookup"><span data-stu-id="0846a-109">countryCode</span></span>    | <span data-ttu-id="0846a-110">String</span><span class="sxs-lookup"><span data-stu-id="0846a-110">String</span></span>                        | <span data-ttu-id="0846a-111">Код страны ISO 3166-1 Alpha-2 в наиболее подсчитанном физическом расположении участника в начале звонка.</span><span class="sxs-lookup"><span data-stu-id="0846a-111">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="0846a-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0846a-112">Read-only.</span></span>                             |
| <span data-ttu-id="0846a-113">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="0846a-113">endpointType</span></span>   | <span data-ttu-id="0846a-114">String</span><span class="sxs-lookup"><span data-stu-id="0846a-114">String</span></span>                        | <span data-ttu-id="0846a-115">Тип конечной точки, используемой участником.</span><span class="sxs-lookup"><span data-stu-id="0846a-115">The type of endpoint the participant is using.</span></span> <span data-ttu-id="0846a-116">Возможные значения: `default`, `skypeForBusiness`, или. `skypeForBusinessVoipPhone`</span><span class="sxs-lookup"><span data-stu-id="0846a-116">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="0846a-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0846a-117">Read-only.</span></span>              |
| <span data-ttu-id="0846a-118">хищения</span><span class="sxs-lookup"><span data-stu-id="0846a-118">identity</span></span>       | [<span data-ttu-id="0846a-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="0846a-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="0846a-120">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="0846a-120">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="0846a-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0846a-121">Read-only.</span></span>                                                                             |
| <span data-ttu-id="0846a-122">languageId</span><span class="sxs-lookup"><span data-stu-id="0846a-122">languageId</span></span>     | <span data-ttu-id="0846a-123">String</span><span class="sxs-lookup"><span data-stu-id="0846a-123">String</span></span>                        | <span data-ttu-id="0846a-124">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="0846a-124">The language culture string.</span></span> <span data-ttu-id="0846a-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0846a-125">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="0846a-126">региональных</span><span class="sxs-lookup"><span data-stu-id="0846a-126">region</span></span>         | <span data-ttu-id="0846a-127">String</span><span class="sxs-lookup"><span data-stu-id="0846a-127">String</span></span>                        | <span data-ttu-id="0846a-128">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="0846a-128">The home region of the participant.</span></span> <span data-ttu-id="0846a-129">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="0846a-129">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="0846a-130">Это не изменяется в зависимости от текущего физического расположения участника, в отличие от countryCode.</span><span class="sxs-lookup"><span data-stu-id="0846a-130">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="0846a-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0846a-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0846a-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0846a-132">JSON representation</span></span>

<span data-ttu-id="0846a-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0846a-133">The following is a JSON representation of the resource.</span></span>

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
