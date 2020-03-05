---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0316cb1bbe474f8265ed384774183759d29aca0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447250"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="a5333-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="a5333-103">participantInfo resource type</span></span>

<span data-ttu-id="a5333-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a5333-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5333-105">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="a5333-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="a5333-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5333-106">Properties</span></span>

| <span data-ttu-id="a5333-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5333-107">Property</span></span>       | <span data-ttu-id="a5333-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a5333-108">Type</span></span>                          | <span data-ttu-id="a5333-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a5333-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a5333-110">хищения</span><span class="sxs-lookup"><span data-stu-id="a5333-110">identity</span></span>       | [<span data-ttu-id="a5333-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5333-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="a5333-112">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="a5333-112">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="a5333-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5333-113">Read-only.</span></span>                                                                             |
| <span data-ttu-id="a5333-114">languageId</span><span class="sxs-lookup"><span data-stu-id="a5333-114">languageId</span></span>     | <span data-ttu-id="a5333-115">String</span><span class="sxs-lookup"><span data-stu-id="a5333-115">String</span></span>                        | <span data-ttu-id="a5333-116">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="a5333-116">The language culture string.</span></span> <span data-ttu-id="a5333-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5333-117">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="a5333-118">региональных</span><span class="sxs-lookup"><span data-stu-id="a5333-118">region</span></span>         | <span data-ttu-id="a5333-119">String</span><span class="sxs-lookup"><span data-stu-id="a5333-119">String</span></span>                        | <span data-ttu-id="a5333-120">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="a5333-120">The home region of the participant.</span></span> <span data-ttu-id="a5333-121">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="a5333-121">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="a5333-122">Это не изменяется в зависимости от текущего физического местоположения участника.</span><span class="sxs-lookup"><span data-stu-id="a5333-122">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="a5333-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5333-123">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a5333-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5333-124">JSON representation</span></span>

<span data-ttu-id="a5333-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5333-125">The following is a JSON representation of the resource.</span></span>

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
