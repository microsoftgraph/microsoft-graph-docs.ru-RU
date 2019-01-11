---
title: Тип ресурса phone
description: Представляет номер телефона.
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805063"
---
# <a name="phone-resource-type"></a><span data-ttu-id="26ccd-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="26ccd-103">phone resource type</span></span>

<span data-ttu-id="26ccd-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="26ccd-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="26ccd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="26ccd-105">Properties</span></span>
| <span data-ttu-id="26ccd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="26ccd-106">Property</span></span>     | <span data-ttu-id="26ccd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="26ccd-107">Type</span></span>   |<span data-ttu-id="26ccd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="26ccd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26ccd-109">number</span><span class="sxs-lookup"><span data-stu-id="26ccd-109">number</span></span>|<span data-ttu-id="26ccd-110">string</span><span class="sxs-lookup"><span data-stu-id="26ccd-110">string</span></span>|<span data-ttu-id="26ccd-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="26ccd-111">The phone number.</span></span>|
|<span data-ttu-id="26ccd-112">type</span><span class="sxs-lookup"><span data-stu-id="26ccd-112">type</span></span>|<span data-ttu-id="26ccd-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="26ccd-113">phoneType</span></span>|<span data-ttu-id="26ccd-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="26ccd-114">The type of phone number.</span></span> <span data-ttu-id="26ccd-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="26ccd-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26ccd-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26ccd-116">JSON representation</span></span>

<span data-ttu-id="26ccd-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26ccd-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
