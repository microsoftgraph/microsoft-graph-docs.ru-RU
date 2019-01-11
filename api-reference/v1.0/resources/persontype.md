---
title: тип ресурса personType
description: Представляет тип пользователя.
localization_priority: Normal
ms.openlocfilehash: d30441a9eab3f51b63e31e5c3c627444312449ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831495"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="ef23f-103">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="ef23f-103">personType resource type</span></span>

<span data-ttu-id="ef23f-104">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef23f-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ef23f-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef23f-105">JSON representation</span></span>

<span data-ttu-id="ef23f-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef23f-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ef23f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef23f-107">Properties</span></span>
| <span data-ttu-id="ef23f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef23f-108">Property</span></span>     | <span data-ttu-id="ef23f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef23f-109">Type</span></span>   |<span data-ttu-id="ef23f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef23f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef23f-111">класс</span><span class="sxs-lookup"><span data-stu-id="ef23f-111">class</span></span>|<span data-ttu-id="ef23f-112">String</span><span class="sxs-lookup"><span data-stu-id="ef23f-112">String</span></span>|<span data-ttu-id="ef23f-113">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="ef23f-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="ef23f-114">subclass</span><span class="sxs-lookup"><span data-stu-id="ef23f-114">subclass</span></span>|<span data-ttu-id="ef23f-115">String</span><span class="sxs-lookup"><span data-stu-id="ef23f-115">String</span></span>|<span data-ttu-id="ef23f-116">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="ef23f-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
