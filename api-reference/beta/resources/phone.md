---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: 162d6a0ccb927c6a48dc01dc3d1e716ab949d89d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812052"
---
# <a name="phone-resource-type"></a><span data-ttu-id="b768f-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="b768f-103">phone resource type</span></span>

<span data-ttu-id="b768f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b768f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b768f-105">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="b768f-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="b768f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b768f-106">Properties</span></span>
| <span data-ttu-id="b768f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b768f-107">Property</span></span>     | <span data-ttu-id="b768f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b768f-108">Type</span></span>   |<span data-ttu-id="b768f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b768f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b768f-110">число</span><span class="sxs-lookup"><span data-stu-id="b768f-110">number</span></span>|<span data-ttu-id="b768f-111">string</span><span class="sxs-lookup"><span data-stu-id="b768f-111">string</span></span>|<span data-ttu-id="b768f-112">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="b768f-112">The phone number.</span></span>|
|<span data-ttu-id="b768f-113">type</span><span class="sxs-lookup"><span data-stu-id="b768f-113">type</span></span>|<span data-ttu-id="b768f-114">String</span><span class="sxs-lookup"><span data-stu-id="b768f-114">String</span></span>|<span data-ttu-id="b768f-115">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="b768f-115">The type of phone number.</span></span> <span data-ttu-id="b768f-116">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="b768f-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b768f-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b768f-117">JSON representation</span></span>

<span data-ttu-id="b768f-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b768f-118">Here is a JSON representation of the resource.</span></span>

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
