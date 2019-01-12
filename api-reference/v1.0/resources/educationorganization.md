---
title: Тип ресурса educationOrganization
description: Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977425"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="9f9da-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="9f9da-103">educationOrganization resource type</span></span>

<span data-ttu-id="9f9da-104">Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.</span><span class="sxs-lookup"><span data-stu-id="9f9da-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="9f9da-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f9da-105">Properties</span></span>
| <span data-ttu-id="9f9da-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f9da-106">Property</span></span>     | <span data-ttu-id="9f9da-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9f9da-107">Type</span></span>   |<span data-ttu-id="9f9da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9f9da-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f9da-109">описание</span><span class="sxs-lookup"><span data-stu-id="9f9da-109">description</span></span>|<span data-ttu-id="9f9da-110">Строка</span><span class="sxs-lookup"><span data-stu-id="9f9da-110">String</span></span>| <span data-ttu-id="9f9da-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="9f9da-111">Organization description.</span></span>|
|<span data-ttu-id="9f9da-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9da-112">displayName</span></span>|<span data-ttu-id="9f9da-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9f9da-113">String</span></span>| <span data-ttu-id="9f9da-114">Отображаемое имя организации.</span><span class="sxs-lookup"><span data-stu-id="9f9da-114">Organization display name.</span></span>|
|<span data-ttu-id="9f9da-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="9f9da-115">externalSource</span></span>|<span data-ttu-id="9f9da-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="9f9da-116">educationExternalSource</span></span>| <span data-ttu-id="9f9da-117">Источник, где был создан данной организации.</span><span class="sxs-lookup"><span data-stu-id="9f9da-117">Source where this organization was created from.</span></span> <span data-ttu-id="9f9da-118">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9f9da-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f9da-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9f9da-119">Relationships</span></span>
<span data-ttu-id="9f9da-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9f9da-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9f9da-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9f9da-121">JSON representation</span></span>

<span data-ttu-id="9f9da-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f9da-122">The following is a JSON representation of the resource.</span></span>

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
