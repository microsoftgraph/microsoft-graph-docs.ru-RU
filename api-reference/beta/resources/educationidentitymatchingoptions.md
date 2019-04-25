---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543246"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="2c805-105">Тип ресурса Едукатионидентитиматчингоптионс</span><span class="sxs-lookup"><span data-stu-id="2c805-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c805-106">Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="2c805-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="2c805-107">Исходное свойство должно существовать в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="2c805-107">The source property should exist in the source data.</span></span> <span data-ttu-id="2c805-108">Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2c805-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="2c805-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c805-109">Properties</span></span>

| <span data-ttu-id="2c805-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c805-110">Property</span></span> | <span data-ttu-id="2c805-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2c805-111">Type</span></span> | <span data-ttu-id="2c805-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2c805-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2c805-113">**Тег**</span><span class="sxs-lookup"><span data-stu-id="2c805-113">**appliesTo**</span></span> | <span data-ttu-id="2c805-114">string</span><span class="sxs-lookup"><span data-stu-id="2c805-114">string</span></span> |  <span data-ttu-id="2c805-115">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="2c805-115">The user role type to assign to the license.</span></span> <span data-ttu-id="2c805-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="2c805-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="2c805-117">**Саурцепропертинаме**</span><span class="sxs-lookup"><span data-stu-id="2c805-117">**sourcePropertyName**</span></span> | <span data-ttu-id="2c805-118">string</span><span class="sxs-lookup"><span data-stu-id="2c805-118">string</span></span> |  <span data-ttu-id="2c805-119">Имя исходного свойства, которое должно быть именем поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="2c805-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="2c805-120">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="2c805-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="2c805-121">**Таржетпропертинаме**</span><span class="sxs-lookup"><span data-stu-id="2c805-121">**targetPropertyName**</span></span> | <span data-ttu-id="2c805-122">string</span><span class="sxs-lookup"><span data-stu-id="2c805-122">string</span></span> |  <span data-ttu-id="2c805-123">Имя целевого свойства, которое должно быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2c805-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="2c805-124">В этом свойстве учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="2c805-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="2c805-125">**Таржетдомаин**</span><span class="sxs-lookup"><span data-stu-id="2c805-125">**targetDomain**</span></span> | <span data-ttu-id="2c805-126">string</span><span class="sxs-lookup"><span data-stu-id="2c805-126">string</span></span> |  <span data-ttu-id="2c805-127">Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="2c805-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="2c805-128">Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.</span><span class="sxs-lookup"><span data-stu-id="2c805-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="2c805-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c805-129">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
