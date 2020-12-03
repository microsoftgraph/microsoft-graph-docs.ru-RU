---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c05222185b87e03c86257939cec098b3ac212e8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522995"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="c8dbf-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="c8dbf-103">participantInfo resource type</span></span>

<span data-ttu-id="c8dbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8dbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8dbf-105">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="c8dbf-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="c8dbf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8dbf-106">Properties</span></span>

| <span data-ttu-id="c8dbf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8dbf-107">Property</span></span>         | <span data-ttu-id="c8dbf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c8dbf-108">Type</span></span>                            | <span data-ttu-id="c8dbf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c8dbf-109">Description</span></span>                                                                                                                                                                                                      |
| :--------------- | :------------------------------ | :-----------------------------------------------------------------------------------------------------------------------------------------------------------                                                     |
| <span data-ttu-id="c8dbf-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="c8dbf-110">countryCode</span></span>      | <span data-ttu-id="c8dbf-111">String</span><span class="sxs-lookup"><span data-stu-id="c8dbf-111">String</span></span>                          | <span data-ttu-id="c8dbf-112">Код страны ISO 3166-1 Alpha-2 в наиболее подсчитанном физическом расположении участника в начале звонка.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="c8dbf-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-113">Read-only.</span></span>                                                                                   |
| <span data-ttu-id="c8dbf-114">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="c8dbf-114">endpointType</span></span>     | <span data-ttu-id="c8dbf-115">String</span><span class="sxs-lookup"><span data-stu-id="c8dbf-115">String</span></span>                          | <span data-ttu-id="c8dbf-116">Тип конечной точки, используемой участником.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="c8dbf-117">Возможные значения: `default` , `skypeForBusiness` , или `skypeForBusinessVoipPhone` .</span><span class="sxs-lookup"><span data-stu-id="c8dbf-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="c8dbf-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-118">Read-only.</span></span>                                                                    |
| <span data-ttu-id="c8dbf-119">хищения</span><span class="sxs-lookup"><span data-stu-id="c8dbf-119">identity</span></span>         | [<span data-ttu-id="c8dbf-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="c8dbf-120">identitySet</span></span>](identityset.md)   | <span data-ttu-id="c8dbf-121">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="c8dbf-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-122">Read-only.</span></span>                                                                                                                                   |
| <span data-ttu-id="c8dbf-123">languageId</span><span class="sxs-lookup"><span data-stu-id="c8dbf-123">languageId</span></span>       | <span data-ttu-id="c8dbf-124">String</span><span class="sxs-lookup"><span data-stu-id="c8dbf-124">String</span></span>                          | <span data-ttu-id="c8dbf-125">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-125">The language culture string.</span></span> <span data-ttu-id="c8dbf-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-126">Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="c8dbf-127">региональных</span><span class="sxs-lookup"><span data-stu-id="c8dbf-127">region</span></span>           | <span data-ttu-id="c8dbf-128">String</span><span class="sxs-lookup"><span data-stu-id="c8dbf-128">String</span></span>                          | <span data-ttu-id="c8dbf-129">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-129">The home region of the participant.</span></span> <span data-ttu-id="c8dbf-130">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="c8dbf-131">Это не изменяется в зависимости от текущего физического расположения участника, в отличие от countryCode.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="c8dbf-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-132">Read-only.</span></span> |
| <span data-ttu-id="c8dbf-133">platformId</span><span class="sxs-lookup"><span data-stu-id="c8dbf-133">platformId</span></span>       | <span data-ttu-id="c8dbf-134">String</span><span class="sxs-lookup"><span data-stu-id="c8dbf-134">String</span></span>                          | <span data-ttu-id="c8dbf-135">Идентификатор клиентской платформы участника.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-135">The client platform ID of the participant.</span></span> <span data-ttu-id="c8dbf-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-136">Read-only.</span></span>    |


## <a name="json-representation"></a><span data-ttu-id="c8dbf-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8dbf-137">JSON representation</span></span>

<span data-ttu-id="c8dbf-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8dbf-138">The following is a JSON representation of the resource.</span></span>

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
  "region": "String",
  "platformId": "String",
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


