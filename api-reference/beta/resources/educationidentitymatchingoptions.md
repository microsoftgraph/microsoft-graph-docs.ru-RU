---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b17ca8548d7a70b8f652ad2d54455fb6040677d
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435028"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="6977f-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="6977f-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="6977f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6977f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6977f-107">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="6977f-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="6977f-108">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="6977f-108">The source property should exist in the source data.</span></span> <span data-ttu-id="6977f-109">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6977f-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="6977f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6977f-110">Properties</span></span>

| <span data-ttu-id="6977f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6977f-111">Property</span></span>           | <span data-ttu-id="6977f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6977f-112">Type</span></span>   | <span data-ttu-id="6977f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6977f-113">Description</span></span>                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6977f-114">Тег</span><span class="sxs-lookup"><span data-stu-id="6977f-114">appliesTo</span></span>          | <span data-ttu-id="6977f-115">String</span><span class="sxs-lookup"><span data-stu-id="6977f-115">String</span></span> | <span data-ttu-id="6977f-116">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="6977f-116">The user role type to assign to the license.</span></span> <span data-ttu-id="6977f-117">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="6977f-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>                                                             |
| <span data-ttu-id="6977f-118">саурцепропертинаме</span><span class="sxs-lookup"><span data-stu-id="6977f-118">sourcePropertyName</span></span> | <span data-ttu-id="6977f-119">Строка</span><span class="sxs-lookup"><span data-stu-id="6977f-119">String</span></span> | <span data-ttu-id="6977f-120">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="6977f-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="6977f-121">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="6977f-121">This property is case-sensitive.</span></span>                                             |
| <span data-ttu-id="6977f-122">таржетпропертинаме</span><span class="sxs-lookup"><span data-stu-id="6977f-122">targetPropertyName</span></span> | <span data-ttu-id="6977f-123">Строка</span><span class="sxs-lookup"><span data-stu-id="6977f-123">String</span></span> | <span data-ttu-id="6977f-124">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6977f-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="6977f-125">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="6977f-125">This property is case-sensitive.</span></span>                                                |
| <span data-ttu-id="6977f-126">таржетдомаин</span><span class="sxs-lookup"><span data-stu-id="6977f-126">targetDomain</span></span>       | <span data-ttu-id="6977f-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6977f-127">String</span></span> | <span data-ttu-id="6977f-128">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="6977f-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="6977f-129">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="6977f-129">If provided as null, the source property will be used to match with the target property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6977f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6977f-130">JSON representation</span></span>

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
