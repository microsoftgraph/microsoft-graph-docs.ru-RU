---
title: Тип ресурса educationOrganization
description: 'Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 015b1c886f439e3c5952d1c1a5fcce02fb21773b
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909655"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="ceff0-103">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="ceff0-103">educationOrganization resource type</span></span>

<span data-ttu-id="ceff0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceff0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceff0-105">Абстрактный объект, используемый для моделирования сходства между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="ceff0-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="ceff0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ceff0-106">Properties</span></span>

| <span data-ttu-id="ceff0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ceff0-107">Property</span></span>       | <span data-ttu-id="ceff0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ceff0-108">Type</span></span>   | <span data-ttu-id="ceff0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ceff0-109">Description</span></span>                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| <span data-ttu-id="ceff0-110">description</span><span class="sxs-lookup"><span data-stu-id="ceff0-110">description</span></span>    | <span data-ttu-id="ceff0-111">String</span><span class="sxs-lookup"><span data-stu-id="ceff0-111">String</span></span> | <span data-ttu-id="ceff0-112">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="ceff0-112">Organization description.</span></span>                                                         |
| <span data-ttu-id="ceff0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ceff0-113">displayName</span></span>    | <span data-ttu-id="ceff0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ceff0-114">String</span></span> | <span data-ttu-id="ceff0-115">Отображаемое имя Организации.</span><span class="sxs-lookup"><span data-stu-id="ceff0-115">Organization display name.</span></span>                                                        |
| <span data-ttu-id="ceff0-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="ceff0-116">externalSource</span></span> | <span data-ttu-id="ceff0-117">String</span><span class="sxs-lookup"><span data-stu-id="ceff0-117">String</span></span> | <span data-ttu-id="ceff0-118">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="ceff0-118">Where this user was created from.</span></span> <span data-ttu-id="ceff0-119">Возможные значения: `sis` , `lms` , или `manual` .</span><span class="sxs-lookup"><span data-stu-id="ceff0-119">Possible values are: `sis`, `lms`, or `manual`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ceff0-120">Связи</span><span class="sxs-lookup"><span data-stu-id="ceff0-120">Relationships</span></span>

<span data-ttu-id="ceff0-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ceff0-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceff0-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ceff0-122">JSON representation</span></span>

<span data-ttu-id="ceff0-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ceff0-123">The following is a JSON representation of the resource.</span></span>

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
