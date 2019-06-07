---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 37ebb55fdd5457841ca0083c18518babca7565c4
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750152"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="f572a-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="f572a-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f572a-106">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="f572a-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="f572a-107">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="f572a-107">The source property should exist in the source data.</span></span> <span data-ttu-id="f572a-108">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f572a-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="f572a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f572a-109">Properties</span></span>

| <span data-ttu-id="f572a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f572a-110">Property</span></span> | <span data-ttu-id="f572a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f572a-111">Type</span></span> | <span data-ttu-id="f572a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f572a-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f572a-113">**Тег**</span><span class="sxs-lookup"><span data-stu-id="f572a-113">**appliesTo**</span></span> | <span data-ttu-id="f572a-114">string</span><span class="sxs-lookup"><span data-stu-id="f572a-114">string</span></span> |  <span data-ttu-id="f572a-115">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="f572a-115">The user role type to assign to the license.</span></span> <span data-ttu-id="f572a-116">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="f572a-116">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="f572a-117">**Саурцепропертинаме**</span><span class="sxs-lookup"><span data-stu-id="f572a-117">**sourcePropertyName**</span></span> | <span data-ttu-id="f572a-118">string</span><span class="sxs-lookup"><span data-stu-id="f572a-118">string</span></span> |  <span data-ttu-id="f572a-119">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="f572a-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="f572a-120">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f572a-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="f572a-121">**Таржетпропертинаме**</span><span class="sxs-lookup"><span data-stu-id="f572a-121">**targetPropertyName**</span></span> | <span data-ttu-id="f572a-122">string</span><span class="sxs-lookup"><span data-stu-id="f572a-122">string</span></span> |  <span data-ttu-id="f572a-123">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f572a-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="f572a-124">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f572a-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="f572a-125">**Таржетдомаин**</span><span class="sxs-lookup"><span data-stu-id="f572a-125">**targetDomain**</span></span> | <span data-ttu-id="f572a-126">string</span><span class="sxs-lookup"><span data-stu-id="f572a-126">string</span></span> |  <span data-ttu-id="f572a-127">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="f572a-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="f572a-128">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="f572a-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="f572a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f572a-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
