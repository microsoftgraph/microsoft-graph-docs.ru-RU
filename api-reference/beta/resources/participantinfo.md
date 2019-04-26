---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568611"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="ef000-103">Тип ресурса ПартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="ef000-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef000-104">Содержит дополнительные свойства удостоверения участника</span><span class="sxs-lookup"><span data-stu-id="ef000-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="ef000-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef000-105">Properties</span></span>

| <span data-ttu-id="ef000-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef000-106">Property</span></span>       | <span data-ttu-id="ef000-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ef000-107">Type</span></span>                          | <span data-ttu-id="ef000-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ef000-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="ef000-109">хищения</span><span class="sxs-lookup"><span data-stu-id="ef000-109">identity</span></span>       | [<span data-ttu-id="ef000-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef000-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="ef000-111">[Удостоверение](identityset.md) , связанное с этим участником.</span><span class="sxs-lookup"><span data-stu-id="ef000-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="ef000-112">languageId</span><span class="sxs-lookup"><span data-stu-id="ef000-112">languageId</span></span>     | <span data-ttu-id="ef000-113">String</span><span class="sxs-lookup"><span data-stu-id="ef000-113">String</span></span>                        | <span data-ttu-id="ef000-114">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="ef000-114">The language culture string.</span></span> |
| <span data-ttu-id="ef000-115">региональных</span><span class="sxs-lookup"><span data-stu-id="ef000-115">region</span></span>         | <span data-ttu-id="ef000-116">String</span><span class="sxs-lookup"><span data-stu-id="ef000-116">String</span></span>                        | <span data-ttu-id="ef000-117">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="ef000-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef000-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef000-118">JSON representation</span></span>

<span data-ttu-id="ef000-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef000-119">The following is a JSON representation of the resource.</span></span>

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
