---
title: Тип ресурса educationOrganization
description: 'Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507476"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="01a8c-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="01a8c-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a8c-104">Использовать для моделирования обеих другой организации типов в образовательных сектора абстрактной сущности.</span><span class="sxs-lookup"><span data-stu-id="01a8c-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="01a8c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="01a8c-105">Properties</span></span>
| <span data-ttu-id="01a8c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a8c-106">Property</span></span>     | <span data-ttu-id="01a8c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="01a8c-107">Type</span></span>   |<span data-ttu-id="01a8c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="01a8c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01a8c-109">description</span><span class="sxs-lookup"><span data-stu-id="01a8c-109">description</span></span>|<span data-ttu-id="01a8c-110">String</span><span class="sxs-lookup"><span data-stu-id="01a8c-110">String</span></span>| <span data-ttu-id="01a8c-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="01a8c-111">Organization description.</span></span>|
|<span data-ttu-id="01a8c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="01a8c-112">displayName</span></span>|<span data-ttu-id="01a8c-113">String</span><span class="sxs-lookup"><span data-stu-id="01a8c-113">String</span></span>| <span data-ttu-id="01a8c-114">Отображаемое имя организации.</span><span class="sxs-lookup"><span data-stu-id="01a8c-114">Organization display name.</span></span>|
|<span data-ttu-id="01a8c-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="01a8c-115">externalSource</span></span>|<span data-ttu-id="01a8c-116">string</span><span class="sxs-lookup"><span data-stu-id="01a8c-116">string</span></span>| <span data-ttu-id="01a8c-117">Источник, где был создан данной организации.</span><span class="sxs-lookup"><span data-stu-id="01a8c-117">Source where this organization was created from.</span></span> <span data-ttu-id="01a8c-118">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="01a8c-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01a8c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="01a8c-119">Relationships</span></span>
<span data-ttu-id="01a8c-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="01a8c-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="01a8c-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01a8c-121">JSON representation</span></span>

<span data-ttu-id="01a8c-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a8c-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
