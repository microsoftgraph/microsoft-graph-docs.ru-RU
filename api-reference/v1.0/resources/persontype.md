---
title: тип ресурса personType
description: Представляет тип пользователя.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917274"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="7a4ad-103">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="7a4ad-103">personType resource type</span></span>

<span data-ttu-id="7a4ad-104">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a4ad-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7a4ad-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a4ad-105">JSON representation</span></span>

<span data-ttu-id="7a4ad-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a4ad-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7a4ad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a4ad-107">Properties</span></span>
| <span data-ttu-id="7a4ad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a4ad-108">Property</span></span>     | <span data-ttu-id="7a4ad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a4ad-109">Type</span></span>   |<span data-ttu-id="7a4ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a4ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a4ad-111">класс</span><span class="sxs-lookup"><span data-stu-id="7a4ad-111">class</span></span>|<span data-ttu-id="7a4ad-112">String</span><span class="sxs-lookup"><span data-stu-id="7a4ad-112">String</span></span>|<span data-ttu-id="7a4ad-113">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="7a4ad-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="7a4ad-114">subclass</span><span class="sxs-lookup"><span data-stu-id="7a4ad-114">subclass</span></span>|<span data-ttu-id="7a4ad-115">String</span><span class="sxs-lookup"><span data-stu-id="7a4ad-115">String</span></span>|<span data-ttu-id="7a4ad-116">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="7a4ad-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
