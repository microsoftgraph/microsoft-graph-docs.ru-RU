---
title: Тип ресурса phone
description: Представляет номер телефона.
localization_priority: Normal
ms.openlocfilehash: a343d4e1d65126048a27ad723c86ae49eb2ed752
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527231"
---
# <a name="phone-resource-type"></a><span data-ttu-id="957ca-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="957ca-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="957ca-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="957ca-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="957ca-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="957ca-105">Properties</span></span>
| <span data-ttu-id="957ca-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="957ca-106">Property</span></span>     | <span data-ttu-id="957ca-107">Тип</span><span class="sxs-lookup"><span data-stu-id="957ca-107">Type</span></span>   |<span data-ttu-id="957ca-108">Описание</span><span class="sxs-lookup"><span data-stu-id="957ca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="957ca-109">number</span><span class="sxs-lookup"><span data-stu-id="957ca-109">number</span></span>|<span data-ttu-id="957ca-110">string</span><span class="sxs-lookup"><span data-stu-id="957ca-110">string</span></span>|<span data-ttu-id="957ca-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="957ca-111">The phone number.</span></span>|
|<span data-ttu-id="957ca-112">type</span><span class="sxs-lookup"><span data-stu-id="957ca-112">type</span></span>|<span data-ttu-id="957ca-113">String</span><span class="sxs-lookup"><span data-stu-id="957ca-113">String</span></span>|<span data-ttu-id="957ca-p101">Тип номера телефона. Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="957ca-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="957ca-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="957ca-116">JSON representation</span></span>

<span data-ttu-id="957ca-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="957ca-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/phone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
