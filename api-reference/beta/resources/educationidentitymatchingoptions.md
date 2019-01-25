---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513706"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="48922-105">Тип ресурса educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="48922-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48922-106">Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="48922-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="48922-107">Свойство source должна существовать в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="48922-107">The source property should exist in the source data.</span></span> <span data-ttu-id="48922-108">Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="48922-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="48922-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="48922-109">Properties</span></span>

| <span data-ttu-id="48922-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="48922-110">Property</span></span> | <span data-ttu-id="48922-111">Тип</span><span class="sxs-lookup"><span data-stu-id="48922-111">Type</span></span> | <span data-ttu-id="48922-112">Описание</span><span class="sxs-lookup"><span data-stu-id="48922-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="48922-113">appliesTo</span><span class="sxs-lookup"><span data-stu-id="48922-113">**appliesTo**</span></span> | <span data-ttu-id="48922-114">string</span><span class="sxs-lookup"><span data-stu-id="48922-114">string</span></span> |  <span data-ttu-id="48922-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="48922-115">The user role type to assign to the license.</span></span> <span data-ttu-id="48922-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="48922-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="48922-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="48922-117">**sourcePropertyName**</span></span> | <span data-ttu-id="48922-118">string</span><span class="sxs-lookup"><span data-stu-id="48922-118">string</span></span> |  <span data-ttu-id="48922-119">Имя свойства источника, которое должно быть имя поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="48922-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="48922-120">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="48922-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="48922-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="48922-121">**targetPropertyName**</span></span> | <span data-ttu-id="48922-122">string</span><span class="sxs-lookup"><span data-stu-id="48922-122">string</span></span> |  <span data-ttu-id="48922-123">Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="48922-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="48922-124">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="48922-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="48922-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="48922-125">**targetDomain**</span></span> | <span data-ttu-id="48922-126">string</span><span class="sxs-lookup"><span data-stu-id="48922-126">string</span></span> |  <span data-ttu-id="48922-127">Домен суффикс со свойством источника для сопоставления в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="48922-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="48922-128">Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="48922-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="48922-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48922-129">JSON representation</span></span>
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
