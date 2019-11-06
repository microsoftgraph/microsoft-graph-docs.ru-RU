---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4cffe361b63ddc6d54d2ad16c29d2de8836044fc
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006594"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="c2911-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="c2911-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2911-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="c2911-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="c2911-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2911-105">Properties</span></span>

| <span data-ttu-id="c2911-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2911-106">Property</span></span>       | <span data-ttu-id="c2911-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c2911-107">Type</span></span>                          | <span data-ttu-id="c2911-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c2911-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="c2911-109">хищения</span><span class="sxs-lookup"><span data-stu-id="c2911-109">identity</span></span>       | [<span data-ttu-id="c2911-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2911-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c2911-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="c2911-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="c2911-112">languageId</span><span class="sxs-lookup"><span data-stu-id="c2911-112">languageId</span></span>     | <span data-ttu-id="c2911-113">String</span><span class="sxs-lookup"><span data-stu-id="c2911-113">String</span></span>                        | <span data-ttu-id="c2911-114">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="c2911-114">The language culture string.</span></span> |
| <span data-ttu-id="c2911-115">региональных</span><span class="sxs-lookup"><span data-stu-id="c2911-115">region</span></span>         | <span data-ttu-id="c2911-116">String</span><span class="sxs-lookup"><span data-stu-id="c2911-116">String</span></span>                        | <span data-ttu-id="c2911-117">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="c2911-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2911-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2911-118">JSON representation</span></span>

<span data-ttu-id="c2911-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2911-119">The following is a JSON representation of the resource.</span></span>

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
