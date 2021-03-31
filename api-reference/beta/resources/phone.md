---
title: тип ресурса телефона
description: Представляет номер телефона.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 00867d2d3725b4dd0607c87771019f85ab1058b6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468851"
---
# <a name="phone-resource-type"></a><span data-ttu-id="a9d35-103">тип ресурса телефона</span><span class="sxs-lookup"><span data-stu-id="a9d35-103">phone resource type</span></span>

<span data-ttu-id="a9d35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9d35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9d35-105">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="a9d35-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="a9d35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9d35-106">Properties</span></span>
| <span data-ttu-id="a9d35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9d35-107">Property</span></span>     | <span data-ttu-id="a9d35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d35-108">Type</span></span>   |<span data-ttu-id="a9d35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a9d35-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9d35-110">число</span><span class="sxs-lookup"><span data-stu-id="a9d35-110">number</span></span>|<span data-ttu-id="a9d35-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d35-111">string</span></span>|<span data-ttu-id="a9d35-112">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="a9d35-112">The phone number.</span></span>|
|<span data-ttu-id="a9d35-113">type</span><span class="sxs-lookup"><span data-stu-id="a9d35-113">type</span></span>|<span data-ttu-id="a9d35-114">String</span><span class="sxs-lookup"><span data-stu-id="a9d35-114">String</span></span>|<span data-ttu-id="a9d35-115">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="a9d35-115">The type of phone number.</span></span> <span data-ttu-id="a9d35-116">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="a9d35-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9d35-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9d35-117">JSON representation</span></span>

<span data-ttu-id="a9d35-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d35-118">Here is a JSON representation of the resource.</span></span>

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


