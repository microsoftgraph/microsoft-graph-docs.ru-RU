---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a28577dca488cb11bc6c34c7c653e0db1ede3d4e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972623"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="3f60d-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="3f60d-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f60d-104">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="3f60d-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="3f60d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f60d-105">Properties</span></span>
| <span data-ttu-id="3f60d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f60d-106">Property</span></span>     | <span data-ttu-id="3f60d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3f60d-107">Type</span></span>   |<span data-ttu-id="3f60d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3f60d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f60d-109">description</span><span class="sxs-lookup"><span data-stu-id="3f60d-109">description</span></span>|<span data-ttu-id="3f60d-110">String</span><span class="sxs-lookup"><span data-stu-id="3f60d-110">String</span></span>| <span data-ttu-id="3f60d-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="3f60d-111">Organization description.</span></span>|
|<span data-ttu-id="3f60d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3f60d-112">displayName</span></span>|<span data-ttu-id="3f60d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3f60d-113">String</span></span>| <span data-ttu-id="3f60d-114">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="3f60d-114">Organization display name.</span></span>|
|<span data-ttu-id="3f60d-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="3f60d-115">externalSource</span></span>|<span data-ttu-id="3f60d-116">string</span><span class="sxs-lookup"><span data-stu-id="3f60d-116">string</span></span>| <span data-ttu-id="3f60d-117">Источник, из которого была создана данная организация.</span><span class="sxs-lookup"><span data-stu-id="3f60d-117">Source where this organization was created from.</span></span> <span data-ttu-id="3f60d-118">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3f60d-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f60d-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f60d-119">Relationships</span></span>
<span data-ttu-id="3f60d-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3f60d-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f60d-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3f60d-121">JSON representation</span></span>

<span data-ttu-id="3f60d-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f60d-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
