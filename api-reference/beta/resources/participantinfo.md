---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9869cf1154735742630edf75ea3e4d5303d45bc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344922"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="a9700-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="a9700-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9700-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="a9700-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="a9700-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9700-105">Properties</span></span>

| <span data-ttu-id="a9700-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9700-106">Property</span></span>       | <span data-ttu-id="a9700-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a9700-107">Type</span></span>                          | <span data-ttu-id="a9700-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a9700-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="a9700-109">хищения</span><span class="sxs-lookup"><span data-stu-id="a9700-109">identity</span></span>       | [<span data-ttu-id="a9700-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9700-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="a9700-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="a9700-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="a9700-112">languageId</span><span class="sxs-lookup"><span data-stu-id="a9700-112">languageId</span></span>     | <span data-ttu-id="a9700-113">String</span><span class="sxs-lookup"><span data-stu-id="a9700-113">String</span></span>                        | <span data-ttu-id="a9700-114">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="a9700-114">The language culture string.</span></span> |
| <span data-ttu-id="a9700-115">региональных</span><span class="sxs-lookup"><span data-stu-id="a9700-115">region</span></span>         | <span data-ttu-id="a9700-116">String</span><span class="sxs-lookup"><span data-stu-id="a9700-116">String</span></span>                        | <span data-ttu-id="a9700-117">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="a9700-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9700-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9700-118">JSON representation</span></span>

<span data-ttu-id="a9700-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9700-119">The following is a JSON representation of the resource.</span></span>

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
