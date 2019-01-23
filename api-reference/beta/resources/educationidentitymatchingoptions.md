---
title: Тип ресурса educationIdentityMatchingOptions
description: Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей. Свойство source должна существовать в источнике данных. Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425794"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="e347e-105">Тип ресурса educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="e347e-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="e347e-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e347e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e347e-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e347e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e347e-108">Содержит сопоставления между свойство source и свойства конечного объекта для сопоставления учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="e347e-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="e347e-109">Свойство source должна существовать в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="e347e-109">The source property should exist in the source data.</span></span> <span data-ttu-id="e347e-110">Свойство target должно быть допустимое свойство в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e347e-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="e347e-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e347e-111">Properties</span></span>

| <span data-ttu-id="e347e-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e347e-112">Property</span></span> | <span data-ttu-id="e347e-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e347e-113">Type</span></span> | <span data-ttu-id="e347e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e347e-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e347e-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="e347e-115">**appliesTo**</span></span> | <span data-ttu-id="e347e-116">string</span><span class="sxs-lookup"><span data-stu-id="e347e-116">string</span></span> |  <span data-ttu-id="e347e-117">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="e347e-117">The user role type to assign to the license.</span></span> <span data-ttu-id="e347e-118">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="e347e-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="e347e-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="e347e-119">**sourcePropertyName**</span></span> | <span data-ttu-id="e347e-120">string</span><span class="sxs-lookup"><span data-stu-id="e347e-120">string</span></span> |  <span data-ttu-id="e347e-121">Имя свойства источника, которое должно быть имя поля в источнике данных.</span><span class="sxs-lookup"><span data-stu-id="e347e-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="e347e-122">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="e347e-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="e347e-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="e347e-123">**targetPropertyName**</span></span> | <span data-ttu-id="e347e-124">string</span><span class="sxs-lookup"><span data-stu-id="e347e-124">string</span></span> |  <span data-ttu-id="e347e-125">Имя свойства для конечного объекта должен быть допустимым свойством в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e347e-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="e347e-126">Это свойство соответствует с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="e347e-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="e347e-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="e347e-127">**targetDomain**</span></span> | <span data-ttu-id="e347e-128">string</span><span class="sxs-lookup"><span data-stu-id="e347e-128">string</span></span> |  <span data-ttu-id="e347e-129">Домен суффикс со свойством источника для сопоставления в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="e347e-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="e347e-130">Если этот параметр указан как значение null, свойство source будет использоваться в соответствии с помощью свойства конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="e347e-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="e347e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e347e-131">JSON representation</span></span>
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
