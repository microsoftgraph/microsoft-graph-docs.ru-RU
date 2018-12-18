---
title: Тип ресурса educationOrganization
description: Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.
author: mmast-msft
ms.openlocfilehash: e4c0f69d63108cc88b88f530e99cbd55b23f49ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326147"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="97bf3-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="97bf3-103">educationOrganization resource type</span></span>

<span data-ttu-id="97bf3-104">Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.</span><span class="sxs-lookup"><span data-stu-id="97bf3-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="97bf3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="97bf3-105">Properties</span></span>
| <span data-ttu-id="97bf3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="97bf3-106">Property</span></span>     | <span data-ttu-id="97bf3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="97bf3-107">Type</span></span>   |<span data-ttu-id="97bf3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="97bf3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97bf3-109">описание</span><span class="sxs-lookup"><span data-stu-id="97bf3-109">description</span></span>|<span data-ttu-id="97bf3-110">Строка</span><span class="sxs-lookup"><span data-stu-id="97bf3-110">String</span></span>| <span data-ttu-id="97bf3-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="97bf3-111">Organization description.</span></span>|
|<span data-ttu-id="97bf3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="97bf3-112">displayName</span></span>|<span data-ttu-id="97bf3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="97bf3-113">String</span></span>| <span data-ttu-id="97bf3-114">Отображаемое имя организации.</span><span class="sxs-lookup"><span data-stu-id="97bf3-114">Organization display name.</span></span>|
|<span data-ttu-id="97bf3-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="97bf3-115">externalSource</span></span>|<span data-ttu-id="97bf3-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="97bf3-116">educationExternalSource</span></span>| <span data-ttu-id="97bf3-117">Источник, где был создан данной организации.</span><span class="sxs-lookup"><span data-stu-id="97bf3-117">Source where this organization was created from.</span></span> <span data-ttu-id="97bf3-118">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="97bf3-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97bf3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="97bf3-119">Relationships</span></span>
<span data-ttu-id="97bf3-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97bf3-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="97bf3-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97bf3-121">JSON representation</span></span>

<span data-ttu-id="97bf3-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97bf3-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->