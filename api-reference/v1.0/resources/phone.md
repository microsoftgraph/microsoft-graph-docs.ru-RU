---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6bdcc4331b14ad7a0e03404781014b66daf55b46
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035478"
---
# <a name="phone-resource-type"></a><span data-ttu-id="67d4c-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="67d4c-103">phone resource type</span></span>

<span data-ttu-id="67d4c-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="67d4c-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="67d4c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="67d4c-105">Properties</span></span>
| <span data-ttu-id="67d4c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="67d4c-106">Property</span></span>     | <span data-ttu-id="67d4c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="67d4c-107">Type</span></span>   |<span data-ttu-id="67d4c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="67d4c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67d4c-109">число</span><span class="sxs-lookup"><span data-stu-id="67d4c-109">number</span></span>|<span data-ttu-id="67d4c-110">string</span><span class="sxs-lookup"><span data-stu-id="67d4c-110">string</span></span>|<span data-ttu-id="67d4c-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="67d4c-111">The phone number.</span></span>|
|<span data-ttu-id="67d4c-112">type</span><span class="sxs-lookup"><span data-stu-id="67d4c-112">type</span></span>|<span data-ttu-id="67d4c-113">Фонетипе</span><span class="sxs-lookup"><span data-stu-id="67d4c-113">phoneType</span></span>|<span data-ttu-id="67d4c-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="67d4c-114">The type of phone number.</span></span> <span data-ttu-id="67d4c-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="67d4c-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67d4c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67d4c-116">JSON representation</span></span>

<span data-ttu-id="67d4c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67d4c-117">Here is a JSON representation of the resource.</span></span>

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
