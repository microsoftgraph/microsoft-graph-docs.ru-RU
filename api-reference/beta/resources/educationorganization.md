---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ae3add0c3541e1617fec6bb71f0e05bb8fdc1b3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016683"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="49323-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="49323-103">educationOrganization resource type</span></span>

<span data-ttu-id="49323-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49323-105">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="49323-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="49323-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="49323-106">Properties</span></span>

| <span data-ttu-id="49323-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="49323-107">Property</span></span>       | <span data-ttu-id="49323-108">Тип</span><span class="sxs-lookup"><span data-stu-id="49323-108">Type</span></span>   | <span data-ttu-id="49323-109">Описание</span><span class="sxs-lookup"><span data-stu-id="49323-109">Description</span></span>                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| <span data-ttu-id="49323-110">description</span><span class="sxs-lookup"><span data-stu-id="49323-110">description</span></span>    | <span data-ttu-id="49323-111">String</span><span class="sxs-lookup"><span data-stu-id="49323-111">String</span></span> | <span data-ttu-id="49323-112">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="49323-112">Organization description.</span></span>                                                         |
| <span data-ttu-id="49323-113">displayName</span><span class="sxs-lookup"><span data-stu-id="49323-113">displayName</span></span>    | <span data-ttu-id="49323-114">String</span><span class="sxs-lookup"><span data-stu-id="49323-114">String</span></span> | <span data-ttu-id="49323-115">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="49323-115">Organization display name.</span></span>                                                        |
| <span data-ttu-id="49323-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="49323-116">externalSource</span></span> | <span data-ttu-id="49323-117">String</span><span class="sxs-lookup"><span data-stu-id="49323-117">String</span></span> | <span data-ttu-id="49323-118">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="49323-118">Where this user was created from.</span></span> <span data-ttu-id="49323-119">Возможные значения: `sis` , `lms` , или `manual` .</span><span class="sxs-lookup"><span data-stu-id="49323-119">Possible values are: `sis`, `lms`, or `manual`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="49323-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="49323-120">Relationships</span></span>

<span data-ttu-id="49323-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49323-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49323-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="49323-122">JSON representation</span></span>

<span data-ttu-id="49323-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49323-123">The following is a JSON representation of the resource.</span></span>

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


