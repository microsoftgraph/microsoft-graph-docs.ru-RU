---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b603d93b2be2fef6a999cf3c1d7663fc7405da9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913732"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="c14c0-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="c14c0-103">participantInfo resource type</span></span>

<span data-ttu-id="c14c0-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="c14c0-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="c14c0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c14c0-105">Properties</span></span>

| <span data-ttu-id="c14c0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c14c0-106">Property</span></span>       | <span data-ttu-id="c14c0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c14c0-107">Type</span></span>                          | <span data-ttu-id="c14c0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c14c0-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c14c0-109">хищения</span><span class="sxs-lookup"><span data-stu-id="c14c0-109">identity</span></span>       | [<span data-ttu-id="c14c0-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c14c0-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c14c0-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="c14c0-111">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="c14c0-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c14c0-112">Read-only.</span></span>                                                                             |
| <span data-ttu-id="c14c0-113">languageId</span><span class="sxs-lookup"><span data-stu-id="c14c0-113">languageId</span></span>     | <span data-ttu-id="c14c0-114">String</span><span class="sxs-lookup"><span data-stu-id="c14c0-114">String</span></span>                        | <span data-ttu-id="c14c0-115">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="c14c0-115">The language culture string.</span></span> <span data-ttu-id="c14c0-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c14c0-116">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="c14c0-117">региональных</span><span class="sxs-lookup"><span data-stu-id="c14c0-117">region</span></span>         | <span data-ttu-id="c14c0-118">String</span><span class="sxs-lookup"><span data-stu-id="c14c0-118">String</span></span>                        | <span data-ttu-id="c14c0-119">Домашняя область участника.</span><span class="sxs-lookup"><span data-stu-id="c14c0-119">The home region of the participant.</span></span> <span data-ttu-id="c14c0-120">Это может быть страна, континент или более крупный географический регион.</span><span class="sxs-lookup"><span data-stu-id="c14c0-120">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="c14c0-121">Это не изменяется в зависимости от текущего физического местоположения участника.</span><span class="sxs-lookup"><span data-stu-id="c14c0-121">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="c14c0-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c14c0-122">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c14c0-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c14c0-123">JSON representation</span></span>

<span data-ttu-id="c14c0-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c14c0-124">The following is a JSON representation of the resource.</span></span>

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
