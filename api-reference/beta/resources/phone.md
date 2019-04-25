---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
ms.openlocfilehash: a343d4e1d65126048a27ad723c86ae49eb2ed752
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573769"
---
# <a name="phone-resource-type"></a><span data-ttu-id="3ec6c-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="3ec6c-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec6c-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="3ec6c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ec6c-105">Properties</span></span>
| <span data-ttu-id="3ec6c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ec6c-106">Property</span></span>     | <span data-ttu-id="3ec6c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3ec6c-107">Type</span></span>   |<span data-ttu-id="3ec6c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ec6c-109">число</span><span class="sxs-lookup"><span data-stu-id="3ec6c-109">number</span></span>|<span data-ttu-id="3ec6c-110">string</span><span class="sxs-lookup"><span data-stu-id="3ec6c-110">string</span></span>|<span data-ttu-id="3ec6c-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-111">The phone number.</span></span>|
|<span data-ttu-id="3ec6c-112">type</span><span class="sxs-lookup"><span data-stu-id="3ec6c-112">type</span></span>|<span data-ttu-id="3ec6c-113">String</span><span class="sxs-lookup"><span data-stu-id="3ec6c-113">String</span></span>|<span data-ttu-id="3ec6c-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-114">The type of phone number.</span></span> <span data-ttu-id="3ec6c-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ec6c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ec6c-116">JSON representation</span></span>

<span data-ttu-id="3ec6c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ec6c-117">Here is a JSON representation of the resource.</span></span>

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
