---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462538"
---
# <a name="phone-resource-type"></a><span data-ttu-id="336aa-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="336aa-103">phone resource type</span></span>

<span data-ttu-id="336aa-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="336aa-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="336aa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="336aa-105">Properties</span></span>
| <span data-ttu-id="336aa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="336aa-106">Property</span></span>     | <span data-ttu-id="336aa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="336aa-107">Type</span></span>   |<span data-ttu-id="336aa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="336aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="336aa-109">number</span><span class="sxs-lookup"><span data-stu-id="336aa-109">number</span></span>|<span data-ttu-id="336aa-110">строка</span><span class="sxs-lookup"><span data-stu-id="336aa-110">string</span></span>|<span data-ttu-id="336aa-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="336aa-111">The phone number.</span></span>|
|<span data-ttu-id="336aa-112">type</span><span class="sxs-lookup"><span data-stu-id="336aa-112">type</span></span>|<span data-ttu-id="336aa-113">Фонетипе</span><span class="sxs-lookup"><span data-stu-id="336aa-113">phoneType</span></span>|<span data-ttu-id="336aa-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="336aa-114">The type of phone number.</span></span> <span data-ttu-id="336aa-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="336aa-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="336aa-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="336aa-116">JSON representation</span></span>

<span data-ttu-id="336aa-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="336aa-117">Here is a JSON representation of the resource.</span></span>

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
