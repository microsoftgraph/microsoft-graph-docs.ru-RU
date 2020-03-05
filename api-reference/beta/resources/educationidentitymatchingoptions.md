---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d722beaac54cbd57c227457a0883b856f6eca4bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501831"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="f5755-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="f5755-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="f5755-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5755-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5755-107">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="f5755-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="f5755-108">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="f5755-108">The source property should exist in the source data.</span></span> <span data-ttu-id="f5755-109">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f5755-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="f5755-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5755-110">Properties</span></span>

| <span data-ttu-id="f5755-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5755-111">Property</span></span> | <span data-ttu-id="f5755-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f5755-112">Type</span></span> | <span data-ttu-id="f5755-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f5755-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f5755-114">**Тег**</span><span class="sxs-lookup"><span data-stu-id="f5755-114">**appliesTo**</span></span> | <span data-ttu-id="f5755-115">строка</span><span class="sxs-lookup"><span data-stu-id="f5755-115">string</span></span> |  <span data-ttu-id="f5755-116">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="f5755-116">The user role type to assign to the license.</span></span> <span data-ttu-id="f5755-117">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="f5755-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="f5755-118">**саурцепропертинаме**</span><span class="sxs-lookup"><span data-stu-id="f5755-118">**sourcePropertyName**</span></span> | <span data-ttu-id="f5755-119">строка</span><span class="sxs-lookup"><span data-stu-id="f5755-119">string</span></span> |  <span data-ttu-id="f5755-120">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="f5755-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="f5755-121">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f5755-121">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="f5755-122">**таржетпропертинаме**</span><span class="sxs-lookup"><span data-stu-id="f5755-122">**targetPropertyName**</span></span> | <span data-ttu-id="f5755-123">строка</span><span class="sxs-lookup"><span data-stu-id="f5755-123">string</span></span> |  <span data-ttu-id="f5755-124">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f5755-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="f5755-125">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f5755-125">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="f5755-126">**таржетдомаин**</span><span class="sxs-lookup"><span data-stu-id="f5755-126">**targetDomain**</span></span> | <span data-ttu-id="f5755-127">строка</span><span class="sxs-lookup"><span data-stu-id="f5755-127">string</span></span> |  <span data-ttu-id="f5755-128">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="f5755-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="f5755-129">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="f5755-129">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="f5755-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5755-130">JSON representation</span></span>
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
