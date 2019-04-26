---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
ms.openlocfilehash: 643b146f95fcc85be530ce7907c872f56033240e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344990"
---
# <a name="phone-resource-type"></a><span data-ttu-id="a4d06-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="a4d06-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d06-104">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="a4d06-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="a4d06-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4d06-105">Properties</span></span>
| <span data-ttu-id="a4d06-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4d06-106">Property</span></span>     | <span data-ttu-id="a4d06-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a4d06-107">Type</span></span>   |<span data-ttu-id="a4d06-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a4d06-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4d06-109">число</span><span class="sxs-lookup"><span data-stu-id="a4d06-109">number</span></span>|<span data-ttu-id="a4d06-110">string</span><span class="sxs-lookup"><span data-stu-id="a4d06-110">string</span></span>|<span data-ttu-id="a4d06-111">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="a4d06-111">The phone number.</span></span>|
|<span data-ttu-id="a4d06-112">type</span><span class="sxs-lookup"><span data-stu-id="a4d06-112">type</span></span>|<span data-ttu-id="a4d06-113">String</span><span class="sxs-lookup"><span data-stu-id="a4d06-113">String</span></span>|<span data-ttu-id="a4d06-114">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="a4d06-114">The type of phone number.</span></span> <span data-ttu-id="a4d06-115">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="a4d06-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4d06-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4d06-116">JSON representation</span></span>

<span data-ttu-id="a4d06-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4d06-117">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
