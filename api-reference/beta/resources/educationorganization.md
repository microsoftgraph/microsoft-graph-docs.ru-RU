---
title: Тип ресурса educationOrganization
description: 'Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  '
author: mmast-msft
ms.openlocfilehash: 54f281de29033418b6acb2f9821c5ebd1eaf4db0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349891"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="725ee-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="725ee-103">educationOrganization resource type</span></span>

> <span data-ttu-id="725ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="725ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="725ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="725ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="725ee-106">Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.</span><span class="sxs-lookup"><span data-stu-id="725ee-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="725ee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="725ee-107">Properties</span></span>
| <span data-ttu-id="725ee-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="725ee-108">Property</span></span>     | <span data-ttu-id="725ee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="725ee-109">Type</span></span>   |<span data-ttu-id="725ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="725ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="725ee-111">описание</span><span class="sxs-lookup"><span data-stu-id="725ee-111">description</span></span>|<span data-ttu-id="725ee-112">Строка</span><span class="sxs-lookup"><span data-stu-id="725ee-112">String</span></span>| <span data-ttu-id="725ee-113">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="725ee-113">Organization description.</span></span>|
|<span data-ttu-id="725ee-114">displayName</span><span class="sxs-lookup"><span data-stu-id="725ee-114">displayName</span></span>|<span data-ttu-id="725ee-115">Строка</span><span class="sxs-lookup"><span data-stu-id="725ee-115">String</span></span>| <span data-ttu-id="725ee-116">Отображаемое имя организации.</span><span class="sxs-lookup"><span data-stu-id="725ee-116">Organization display name.</span></span>|
|<span data-ttu-id="725ee-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="725ee-117">externalSource</span></span>|<span data-ttu-id="725ee-118">string</span><span class="sxs-lookup"><span data-stu-id="725ee-118">string</span></span>| <span data-ttu-id="725ee-119">Источник, где был создан данной организации.</span><span class="sxs-lookup"><span data-stu-id="725ee-119">Source where this organization was created from.</span></span> <span data-ttu-id="725ee-120">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="725ee-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="725ee-121">Связи</span><span class="sxs-lookup"><span data-stu-id="725ee-121">Relationships</span></span>
<span data-ttu-id="725ee-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="725ee-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="725ee-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="725ee-123">JSON representation</span></span>

<span data-ttu-id="725ee-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="725ee-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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