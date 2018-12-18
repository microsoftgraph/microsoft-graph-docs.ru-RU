---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
ms.openlocfilehash: bc2b99654d8e27d52ed92d9b55a32fdff8e730f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325433"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="fd387-105">Тип ресурса educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="fd387-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="fd387-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd387-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd387-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd387-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd387-108">Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="fd387-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="fd387-109">Свойство source должна существовать в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="fd387-109">The source property should exist in the source data.</span></span> <span data-ttu-id="fd387-110">Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fd387-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="fd387-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd387-111">Properties</span></span>

| <span data-ttu-id="fd387-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd387-112">Property</span></span> | <span data-ttu-id="fd387-113">Тип</span><span class="sxs-lookup"><span data-stu-id="fd387-113">Type</span></span> | <span data-ttu-id="fd387-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fd387-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fd387-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="fd387-115">**appliesTo**</span></span> | <span data-ttu-id="fd387-116">string</span><span class="sxs-lookup"><span data-stu-id="fd387-116">string</span></span> |  <span data-ttu-id="fd387-117">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="fd387-117">The user role type to assign to the license.</span></span> <span data-ttu-id="fd387-118">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="fd387-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="fd387-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="fd387-119">**sourcePropertyName**</span></span> | <span data-ttu-id="fd387-120">string</span><span class="sxs-lookup"><span data-stu-id="fd387-120">string</span></span> |  <span data-ttu-id="fd387-121">Имя свойства источника, которое должно быть имя поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="fd387-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="fd387-122">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="fd387-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="fd387-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="fd387-123">**targetPropertyName**</span></span> | <span data-ttu-id="fd387-124">string</span><span class="sxs-lookup"><span data-stu-id="fd387-124">string</span></span> |  <span data-ttu-id="fd387-125">Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd387-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="fd387-126">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="fd387-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="fd387-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="fd387-127">**targetDomain**</span></span> | <span data-ttu-id="fd387-128">string</span><span class="sxs-lookup"><span data-stu-id="fd387-128">string</span></span> |  <span data-ttu-id="fd387-129">Домен суффикс со свойством источника для сопоставления в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="fd387-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="fd387-130">Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="fd387-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="fd387-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd387-131">JSON representation</span></span>
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
