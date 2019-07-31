---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88a22ff446aaa4fd1e7093ec507372c03afcc42b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972693"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="b920d-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="b920d-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b920d-106">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="b920d-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="b920d-107">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="b920d-107">The source property should exist in the source data.</span></span> <span data-ttu-id="b920d-108">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b920d-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b920d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b920d-109">Properties</span></span>

| <span data-ttu-id="b920d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b920d-110">Property</span></span> | <span data-ttu-id="b920d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b920d-111">Type</span></span> | <span data-ttu-id="b920d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b920d-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b920d-113">**Тег**</span><span class="sxs-lookup"><span data-stu-id="b920d-113">**appliesTo**</span></span> | <span data-ttu-id="b920d-114">string</span><span class="sxs-lookup"><span data-stu-id="b920d-114">string</span></span> |  <span data-ttu-id="b920d-115">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="b920d-115">The user role type to assign to the license.</span></span> <span data-ttu-id="b920d-116">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="b920d-116">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="b920d-117">**Саурцепропертинаме**</span><span class="sxs-lookup"><span data-stu-id="b920d-117">**sourcePropertyName**</span></span> | <span data-ttu-id="b920d-118">string</span><span class="sxs-lookup"><span data-stu-id="b920d-118">string</span></span> |  <span data-ttu-id="b920d-119">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="b920d-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="b920d-120">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="b920d-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="b920d-121">**Таржетпропертинаме**</span><span class="sxs-lookup"><span data-stu-id="b920d-121">**targetPropertyName**</span></span> | <span data-ttu-id="b920d-122">string</span><span class="sxs-lookup"><span data-stu-id="b920d-122">string</span></span> |  <span data-ttu-id="b920d-123">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b920d-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="b920d-124">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="b920d-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="b920d-125">**Таржетдомаин**</span><span class="sxs-lookup"><span data-stu-id="b920d-125">**targetDomain**</span></span> | <span data-ttu-id="b920d-126">string</span><span class="sxs-lookup"><span data-stu-id="b920d-126">string</span></span> |  <span data-ttu-id="b920d-127">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="b920d-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="b920d-128">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="b920d-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="b920d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b920d-129">JSON representation</span></span>
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
