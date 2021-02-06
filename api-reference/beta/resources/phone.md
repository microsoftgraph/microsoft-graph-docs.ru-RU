---
title: Тип ресурса phone
description: Представляет номер телефона.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 7c6ee74a588540470ceeffcc37b51e29e7e4f597
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130882"
---
# <a name="phone-resource-type"></a><span data-ttu-id="21eb4-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="21eb4-103">phone resource type</span></span>

<span data-ttu-id="21eb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21eb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21eb4-105">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="21eb4-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="21eb4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="21eb4-106">Properties</span></span>
| <span data-ttu-id="21eb4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="21eb4-107">Property</span></span>     | <span data-ttu-id="21eb4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="21eb4-108">Type</span></span>   |<span data-ttu-id="21eb4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21eb4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21eb4-110">число</span><span class="sxs-lookup"><span data-stu-id="21eb4-110">number</span></span>|<span data-ttu-id="21eb4-111">string</span><span class="sxs-lookup"><span data-stu-id="21eb4-111">string</span></span>|<span data-ttu-id="21eb4-112">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="21eb4-112">The phone number.</span></span>|
|<span data-ttu-id="21eb4-113">type</span><span class="sxs-lookup"><span data-stu-id="21eb4-113">type</span></span>|<span data-ttu-id="21eb4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="21eb4-114">String</span></span>|<span data-ttu-id="21eb4-115">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="21eb4-115">The type of phone number.</span></span> <span data-ttu-id="21eb4-116">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="21eb4-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21eb4-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="21eb4-117">JSON representation</span></span>

<span data-ttu-id="21eb4-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21eb4-118">Here is a JSON representation of the resource.</span></span>

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


