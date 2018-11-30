---
title: Тип ресурса phone
description: Представляет номер телефона.
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027385"
---
# <a name="phone-resource-type"></a><span data-ttu-id="d93a7-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="d93a7-103">phone resource type</span></span>

<span data-ttu-id="d93a7-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="d93a7-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="d93a7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d93a7-105">Properties</span></span>
| <span data-ttu-id="d93a7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d93a7-106">Property</span></span>     | <span data-ttu-id="d93a7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d93a7-107">Type</span></span>   |<span data-ttu-id="d93a7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d93a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d93a7-109">number</span><span class="sxs-lookup"><span data-stu-id="d93a7-109">number</span></span>|<span data-ttu-id="d93a7-110">string</span><span class="sxs-lookup"><span data-stu-id="d93a7-110">string</span></span>|<span data-ttu-id="d93a7-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="d93a7-111">The phone number.</span></span>|
|<span data-ttu-id="d93a7-112">type</span><span class="sxs-lookup"><span data-stu-id="d93a7-112">type</span></span>|<span data-ttu-id="d93a7-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="d93a7-113">phoneType</span></span>|<span data-ttu-id="d93a7-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="d93a7-114">The type of phone number.</span></span> <span data-ttu-id="d93a7-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="d93a7-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d93a7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d93a7-116">JSON representation</span></span>

<span data-ttu-id="d93a7-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d93a7-117">Here is a JSON representation of the resource.</span></span>

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
