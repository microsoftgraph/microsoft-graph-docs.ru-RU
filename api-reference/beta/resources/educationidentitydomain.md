---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4e23a9111d2515234d1aa665f4847d732dc563
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435042"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="204e2-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="204e2-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="204e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="204e2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="204e2-106">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="204e2-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="204e2-107">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="204e2-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="204e2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="204e2-108">Properties</span></span>

| <span data-ttu-id="204e2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="204e2-109">Property</span></span>  | <span data-ttu-id="204e2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="204e2-110">Type</span></span>   | <span data-ttu-id="204e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="204e2-111">Description</span></span>                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="204e2-112">Тег</span><span class="sxs-lookup"><span data-stu-id="204e2-112">appliesTo</span></span> | <span data-ttu-id="204e2-113">String</span><span class="sxs-lookup"><span data-stu-id="204e2-113">String</span></span> | <span data-ttu-id="204e2-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="204e2-114">The user role type to assign to the license.</span></span> <span data-ttu-id="204e2-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="204e2-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="204e2-116">name</span><span class="sxs-lookup"><span data-stu-id="204e2-116">name</span></span>      | <span data-ttu-id="204e2-117">String</span><span class="sxs-lookup"><span data-stu-id="204e2-117">String</span></span> | <span data-ttu-id="204e2-118">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="204e2-118">Represents the domain for the user account.</span></span>                                                        |

## <a name="json-representation"></a><span data-ttu-id="204e2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="204e2-119">JSON representation</span></span>

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
