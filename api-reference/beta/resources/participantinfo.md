---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad73ce0bbeaa02b0207f11bbd3f0004857d90506
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966229"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="e57af-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="e57af-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e57af-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="e57af-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="e57af-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e57af-105">Properties</span></span>

| <span data-ttu-id="e57af-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e57af-106">Property</span></span>       | <span data-ttu-id="e57af-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e57af-107">Type</span></span>                          | <span data-ttu-id="e57af-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e57af-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="e57af-109">хищения</span><span class="sxs-lookup"><span data-stu-id="e57af-109">identity</span></span>       | [<span data-ttu-id="e57af-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="e57af-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="e57af-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="e57af-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="e57af-112">languageId</span><span class="sxs-lookup"><span data-stu-id="e57af-112">languageId</span></span>     | <span data-ttu-id="e57af-113">String</span><span class="sxs-lookup"><span data-stu-id="e57af-113">String</span></span>                        | <span data-ttu-id="e57af-114">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="e57af-114">The language culture string.</span></span> |
| <span data-ttu-id="e57af-115">региональных</span><span class="sxs-lookup"><span data-stu-id="e57af-115">region</span></span>         | <span data-ttu-id="e57af-116">String</span><span class="sxs-lookup"><span data-stu-id="e57af-116">String</span></span>                        | <span data-ttu-id="e57af-117">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="e57af-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e57af-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e57af-118">JSON representation</span></span>

<span data-ttu-id="e57af-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e57af-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
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
