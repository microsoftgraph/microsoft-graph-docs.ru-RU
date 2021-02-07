---
title: Тип ресурса phone
description: Представляет номер телефона.
localization_priority: Normal
author: davidmu1
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 703a24bc0b2d1453b210f739573f4b9629355a64
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135732"
---
# <a name="phone-resource-type"></a><span data-ttu-id="27f1d-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="27f1d-103">phone resource type</span></span>

<span data-ttu-id="27f1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27f1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27f1d-105">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="27f1d-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="27f1d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f1d-106">Properties</span></span>
| <span data-ttu-id="27f1d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f1d-107">Property</span></span>     | <span data-ttu-id="27f1d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="27f1d-108">Type</span></span>   |<span data-ttu-id="27f1d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27f1d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27f1d-110">число</span><span class="sxs-lookup"><span data-stu-id="27f1d-110">number</span></span>|<span data-ttu-id="27f1d-111">string</span><span class="sxs-lookup"><span data-stu-id="27f1d-111">string</span></span>|<span data-ttu-id="27f1d-112">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="27f1d-112">The phone number.</span></span>|
|<span data-ttu-id="27f1d-113">type</span><span class="sxs-lookup"><span data-stu-id="27f1d-113">type</span></span>|<span data-ttu-id="27f1d-114">phoneType</span><span class="sxs-lookup"><span data-stu-id="27f1d-114">phoneType</span></span>|<span data-ttu-id="27f1d-115">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="27f1d-115">The type of phone number.</span></span> <span data-ttu-id="27f1d-116">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="27f1d-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27f1d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f1d-117">JSON representation</span></span>

<span data-ttu-id="27f1d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f1d-118">Here is a JSON representation of the resource.</span></span>

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

