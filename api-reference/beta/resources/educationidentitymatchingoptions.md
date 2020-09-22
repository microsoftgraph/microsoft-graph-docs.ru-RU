---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 73c97b0e9c23c455b3e15ed656060eca7f8a3e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095382"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="d5ab5-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="d5ab5-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="d5ab5-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5ab5-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5ab5-107">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="d5ab5-108">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-108">The source property should exist in the source data.</span></span> <span data-ttu-id="d5ab5-109">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d5ab5-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="d5ab5-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5ab5-110">Properties</span></span>

| <span data-ttu-id="d5ab5-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5ab5-111">Property</span></span>           | <span data-ttu-id="d5ab5-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d5ab5-112">Type</span></span>   | <span data-ttu-id="d5ab5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d5ab5-113">Description</span></span>                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d5ab5-114">Тег</span><span class="sxs-lookup"><span data-stu-id="d5ab5-114">appliesTo</span></span>          | <span data-ttu-id="d5ab5-115">String</span><span class="sxs-lookup"><span data-stu-id="d5ab5-115">String</span></span> | <span data-ttu-id="d5ab5-116">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-116">The user role type to assign to the license.</span></span> <span data-ttu-id="d5ab5-117">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>                                                             |
| <span data-ttu-id="d5ab5-118">саурцепропертинаме</span><span class="sxs-lookup"><span data-stu-id="d5ab5-118">sourcePropertyName</span></span> | <span data-ttu-id="d5ab5-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d5ab5-119">String</span></span> | <span data-ttu-id="d5ab5-120">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="d5ab5-121">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-121">This property is case-sensitive.</span></span>                                             |
| <span data-ttu-id="d5ab5-122">таржетпропертинаме</span><span class="sxs-lookup"><span data-stu-id="d5ab5-122">targetPropertyName</span></span> | <span data-ttu-id="d5ab5-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d5ab5-123">String</span></span> | <span data-ttu-id="d5ab5-124">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="d5ab5-125">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-125">This property is case-sensitive.</span></span>                                                |
| <span data-ttu-id="d5ab5-126">таржетдомаин</span><span class="sxs-lookup"><span data-stu-id="d5ab5-126">targetDomain</span></span>       | <span data-ttu-id="d5ab5-127">Строка</span><span class="sxs-lookup"><span data-stu-id="d5ab5-127">String</span></span> | <span data-ttu-id="d5ab5-128">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="d5ab5-129">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="d5ab5-129">If provided as null, the source property will be used to match with the target property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d5ab5-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5ab5-130">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```


