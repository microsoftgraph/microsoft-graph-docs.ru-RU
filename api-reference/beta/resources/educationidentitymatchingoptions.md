---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80e9222f8f0c03294a947f403b33cc4f2cd2ef0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876281"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="881c4-105">Тип ресурса educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="881c4-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="881c4-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="881c4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="881c4-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="881c4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="881c4-108">Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="881c4-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="881c4-109">Свойство source должна существовать в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="881c4-109">The source property should exist in the source data.</span></span> <span data-ttu-id="881c4-110">Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="881c4-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="881c4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="881c4-111">Properties</span></span>

| <span data-ttu-id="881c4-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="881c4-112">Property</span></span> | <span data-ttu-id="881c4-113">Тип</span><span class="sxs-lookup"><span data-stu-id="881c4-113">Type</span></span> | <span data-ttu-id="881c4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="881c4-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="881c4-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="881c4-115">**appliesTo**</span></span> | <span data-ttu-id="881c4-116">string</span><span class="sxs-lookup"><span data-stu-id="881c4-116">string</span></span> |  <span data-ttu-id="881c4-117">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="881c4-117">The user role type to assign to the license.</span></span> <span data-ttu-id="881c4-118">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="881c4-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="881c4-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="881c4-119">**sourcePropertyName**</span></span> | <span data-ttu-id="881c4-120">string</span><span class="sxs-lookup"><span data-stu-id="881c4-120">string</span></span> |  <span data-ttu-id="881c4-121">Имя свойства источника, которое должно быть имя поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="881c4-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="881c4-122">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="881c4-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="881c4-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="881c4-123">**targetPropertyName**</span></span> | <span data-ttu-id="881c4-124">string</span><span class="sxs-lookup"><span data-stu-id="881c4-124">string</span></span> |  <span data-ttu-id="881c4-125">Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="881c4-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="881c4-126">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="881c4-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="881c4-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="881c4-127">**targetDomain**</span></span> | <span data-ttu-id="881c4-128">string</span><span class="sxs-lookup"><span data-stu-id="881c4-128">string</span></span> |  <span data-ttu-id="881c4-129">Домен суффикс со свойством источника для сопоставления в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="881c4-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="881c4-130">Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="881c4-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="881c4-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="881c4-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
