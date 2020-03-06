---
title: Тип ресурса educationOrganization
description: Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a6e32f7bf9c635423ca1aace92aea160f6cc2706
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531527"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="4c118-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="4c118-103">educationOrganization resource type</span></span>

<span data-ttu-id="4c118-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c118-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c118-105">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="4c118-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="4c118-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c118-106">Properties</span></span>
| <span data-ttu-id="4c118-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c118-107">Property</span></span>     | <span data-ttu-id="4c118-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4c118-108">Type</span></span>   |<span data-ttu-id="4c118-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4c118-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c118-110">description</span><span class="sxs-lookup"><span data-stu-id="4c118-110">description</span></span>|<span data-ttu-id="4c118-111">String</span><span class="sxs-lookup"><span data-stu-id="4c118-111">String</span></span>| <span data-ttu-id="4c118-112">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="4c118-112">Organization description.</span></span>|
|<span data-ttu-id="4c118-113">displayName</span><span class="sxs-lookup"><span data-stu-id="4c118-113">displayName</span></span>|<span data-ttu-id="4c118-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4c118-114">String</span></span>| <span data-ttu-id="4c118-115">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="4c118-115">Organization display name.</span></span>|
|<span data-ttu-id="4c118-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="4c118-116">externalSource</span></span>|<span data-ttu-id="4c118-117">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="4c118-117">educationExternalSource</span></span>| <span data-ttu-id="4c118-118">Источник, из которого была создана данная организация.</span><span class="sxs-lookup"><span data-stu-id="4c118-118">Source where this organization was created from.</span></span> <span data-ttu-id="4c118-119">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4c118-119">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c118-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="4c118-120">Relationships</span></span>
<span data-ttu-id="4c118-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4c118-121">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4c118-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4c118-122">JSON representation</span></span>

<span data-ttu-id="4c118-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c118-123">The following is a JSON representation of the resource.</span></span>

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
