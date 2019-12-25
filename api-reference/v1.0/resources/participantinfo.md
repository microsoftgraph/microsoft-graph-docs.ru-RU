---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1dcc164769c2e8168be5f593c35cd62218254add
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871385"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="2605a-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="2605a-103">participantInfo resource type</span></span>

<span data-ttu-id="2605a-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="2605a-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="2605a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2605a-105">Properties</span></span>

| <span data-ttu-id="2605a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2605a-106">Property</span></span>       | <span data-ttu-id="2605a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2605a-107">Type</span></span>                          | <span data-ttu-id="2605a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2605a-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2605a-109">хищения</span><span class="sxs-lookup"><span data-stu-id="2605a-109">identity</span></span>       | [<span data-ttu-id="2605a-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="2605a-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="2605a-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="2605a-111">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="2605a-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2605a-112">Read-only.</span></span>                                                                             |
| <span data-ttu-id="2605a-113">languageId</span><span class="sxs-lookup"><span data-stu-id="2605a-113">languageId</span></span>     | <span data-ttu-id="2605a-114">String</span><span class="sxs-lookup"><span data-stu-id="2605a-114">String</span></span>                        | <span data-ttu-id="2605a-115">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="2605a-115">The language culture string.</span></span> <span data-ttu-id="2605a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2605a-116">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="2605a-117">региональных</span><span class="sxs-lookup"><span data-stu-id="2605a-117">region</span></span>         | <span data-ttu-id="2605a-118">String</span><span class="sxs-lookup"><span data-stu-id="2605a-118">String</span></span>                        | <span data-ttu-id="2605a-119">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="2605a-119">The home region of the participant.</span></span> <span data-ttu-id="2605a-120">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="2605a-120">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="2605a-121">Это не изменяется в зависимости от текущего физического местоположения участника.</span><span class="sxs-lookup"><span data-stu-id="2605a-121">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="2605a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2605a-122">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2605a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2605a-123">JSON representation</span></span>

<span data-ttu-id="2605a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2605a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
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
