---
title: тип ресурса personType
description: Представляет тип пользователя.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 36310a469c5ed9289637f9701ce983db12b14fbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035492"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="bfafa-103">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="bfafa-103">personType resource type</span></span>

<span data-ttu-id="bfafa-104">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="bfafa-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bfafa-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfafa-105">JSON representation</span></span>

<span data-ttu-id="bfafa-106">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfafa-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bfafa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfafa-107">Properties</span></span>
| <span data-ttu-id="bfafa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfafa-108">Property</span></span>     | <span data-ttu-id="bfafa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfafa-109">Type</span></span>   |<span data-ttu-id="bfafa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfafa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfafa-111">класс</span><span class="sxs-lookup"><span data-stu-id="bfafa-111">class</span></span>|<span data-ttu-id="bfafa-112">String</span><span class="sxs-lookup"><span data-stu-id="bfafa-112">String</span></span>|<span data-ttu-id="bfafa-113">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="bfafa-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="bfafa-114">subclass</span><span class="sxs-lookup"><span data-stu-id="bfafa-114">subclass</span></span>|<span data-ttu-id="bfafa-115">String</span><span class="sxs-lookup"><span data-stu-id="bfafa-115">String</span></span>|<span data-ttu-id="bfafa-116">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="bfafa-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
