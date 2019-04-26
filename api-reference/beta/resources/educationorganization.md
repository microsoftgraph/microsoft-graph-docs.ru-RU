---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49afe12f4897df80ce78ba28a024883cefeb0a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340486"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e5de2-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="e5de2-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5de2-104">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="e5de2-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="e5de2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5de2-105">Properties</span></span>
| <span data-ttu-id="e5de2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5de2-106">Property</span></span>     | <span data-ttu-id="e5de2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e5de2-107">Type</span></span>   |<span data-ttu-id="e5de2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e5de2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5de2-109">description</span><span class="sxs-lookup"><span data-stu-id="e5de2-109">description</span></span>|<span data-ttu-id="e5de2-110">String</span><span class="sxs-lookup"><span data-stu-id="e5de2-110">String</span></span>| <span data-ttu-id="e5de2-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="e5de2-111">Organization description.</span></span>|
|<span data-ttu-id="e5de2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e5de2-112">displayName</span></span>|<span data-ttu-id="e5de2-113">String</span><span class="sxs-lookup"><span data-stu-id="e5de2-113">String</span></span>| <span data-ttu-id="e5de2-114">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="e5de2-114">Organization display name.</span></span>|
|<span data-ttu-id="e5de2-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="e5de2-115">externalSource</span></span>|<span data-ttu-id="e5de2-116">string</span><span class="sxs-lookup"><span data-stu-id="e5de2-116">string</span></span>| <span data-ttu-id="e5de2-117">Источник, из которого была создана данная организация.</span><span class="sxs-lookup"><span data-stu-id="e5de2-117">Source where this organization was created from.</span></span> <span data-ttu-id="e5de2-118">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e5de2-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5de2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e5de2-119">Relationships</span></span>
<span data-ttu-id="e5de2-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5de2-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5de2-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5de2-121">JSON representation</span></span>

<span data-ttu-id="e5de2-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5de2-122">The following is a JSON representation of the resource.</span></span>

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
