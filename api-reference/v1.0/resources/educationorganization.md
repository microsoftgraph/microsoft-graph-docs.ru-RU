---
title: Тип ресурса educationOrganization
description: Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c62e65ffb6c6a0e3a8af92bda6a8b1e1c241ada7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032636"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="73120-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="73120-103">educationOrganization resource type</span></span>

<span data-ttu-id="73120-104">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="73120-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="73120-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="73120-105">Properties</span></span>
| <span data-ttu-id="73120-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="73120-106">Property</span></span>     | <span data-ttu-id="73120-107">Тип</span><span class="sxs-lookup"><span data-stu-id="73120-107">Type</span></span>   |<span data-ttu-id="73120-108">Описание</span><span class="sxs-lookup"><span data-stu-id="73120-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73120-109">description</span><span class="sxs-lookup"><span data-stu-id="73120-109">description</span></span>|<span data-ttu-id="73120-110">String</span><span class="sxs-lookup"><span data-stu-id="73120-110">String</span></span>| <span data-ttu-id="73120-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="73120-111">Organization description.</span></span>|
|<span data-ttu-id="73120-112">displayName</span><span class="sxs-lookup"><span data-stu-id="73120-112">displayName</span></span>|<span data-ttu-id="73120-113">Строка</span><span class="sxs-lookup"><span data-stu-id="73120-113">String</span></span>| <span data-ttu-id="73120-114">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="73120-114">Organization display name.</span></span>|
|<span data-ttu-id="73120-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="73120-115">externalSource</span></span>|<span data-ttu-id="73120-116">Едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="73120-116">educationExternalSource</span></span>| <span data-ttu-id="73120-117">Источник, из которого была создана данная организация.</span><span class="sxs-lookup"><span data-stu-id="73120-117">Source where this organization was created from.</span></span> <span data-ttu-id="73120-118">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="73120-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73120-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="73120-119">Relationships</span></span>
<span data-ttu-id="73120-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73120-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="73120-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="73120-121">JSON representation</span></span>

<span data-ttu-id="73120-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73120-122">The following is a JSON representation of the resource.</span></span>

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
