---
title: Тип ресурса educationOrganization
description: Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562806"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="f1468-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="f1468-103">educationOrganization resource type</span></span>

<span data-ttu-id="f1468-104">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="f1468-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="f1468-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1468-105">Properties</span></span>
| <span data-ttu-id="f1468-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1468-106">Property</span></span>     | <span data-ttu-id="f1468-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f1468-107">Type</span></span>   |<span data-ttu-id="f1468-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f1468-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1468-109">description</span><span class="sxs-lookup"><span data-stu-id="f1468-109">description</span></span>|<span data-ttu-id="f1468-110">String</span><span class="sxs-lookup"><span data-stu-id="f1468-110">String</span></span>| <span data-ttu-id="f1468-111">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="f1468-111">Organization description.</span></span>|
|<span data-ttu-id="f1468-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f1468-112">displayName</span></span>|<span data-ttu-id="f1468-113">String</span><span class="sxs-lookup"><span data-stu-id="f1468-113">String</span></span>| <span data-ttu-id="f1468-114">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="f1468-114">Organization display name.</span></span>|
|<span data-ttu-id="f1468-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="f1468-115">externalSource</span></span>|<span data-ttu-id="f1468-116">Едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="f1468-116">educationExternalSource</span></span>| <span data-ttu-id="f1468-117">Источник, из которого была создана данная организация.</span><span class="sxs-lookup"><span data-stu-id="f1468-117">Source where this organization was created from.</span></span> <span data-ttu-id="f1468-118">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f1468-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1468-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f1468-119">Relationships</span></span>
<span data-ttu-id="f1468-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1468-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f1468-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1468-121">JSON representation</span></span>

<span data-ttu-id="f1468-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1468-122">The following is a JSON representation of the resource.</span></span>

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
