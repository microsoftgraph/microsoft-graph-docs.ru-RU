---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b25f935ae404a243826a14c310a17ad80c598380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095393"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="26934-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="26934-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="26934-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26934-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26934-106">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="26934-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="26934-107">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26934-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26934-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26934-108">Properties</span></span>

| <span data-ttu-id="26934-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26934-109">Property</span></span>  | <span data-ttu-id="26934-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26934-110">Type</span></span>   | <span data-ttu-id="26934-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26934-111">Description</span></span>                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="26934-112">Тег</span><span class="sxs-lookup"><span data-stu-id="26934-112">appliesTo</span></span> | <span data-ttu-id="26934-113">String</span><span class="sxs-lookup"><span data-stu-id="26934-113">String</span></span> | <span data-ttu-id="26934-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="26934-114">The user role type to assign to the license.</span></span> <span data-ttu-id="26934-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="26934-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="26934-116">name</span><span class="sxs-lookup"><span data-stu-id="26934-116">name</span></span>      | <span data-ttu-id="26934-117">String</span><span class="sxs-lookup"><span data-stu-id="26934-117">String</span></span> | <span data-ttu-id="26934-118">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="26934-118">Represents the domain for the user account.</span></span>                                                        |

## <a name="json-representation"></a><span data-ttu-id="26934-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26934-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```


