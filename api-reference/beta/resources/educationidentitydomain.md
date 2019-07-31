---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86e65d46c8037ebcbb2c98f9f9e93f94f34bbdef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972707"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="cd10e-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="cd10e-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd10e-105">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd10e-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="cd10e-106">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd10e-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="cd10e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd10e-107">Properties</span></span>

| <span data-ttu-id="cd10e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd10e-108">Property</span></span> | <span data-ttu-id="cd10e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd10e-109">Type</span></span> | <span data-ttu-id="cd10e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd10e-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cd10e-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="cd10e-111">**appliesTo**</span></span> | <span data-ttu-id="cd10e-112">string</span><span class="sxs-lookup"><span data-stu-id="cd10e-112">string</span></span> |  <span data-ttu-id="cd10e-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="cd10e-113">The user role type to assign to the license.</span></span> <span data-ttu-id="cd10e-114">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="cd10e-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="cd10e-115">**name**</span><span class="sxs-lookup"><span data-stu-id="cd10e-115">**name**</span></span> | <span data-ttu-id="cd10e-116">string</span><span class="sxs-lookup"><span data-stu-id="cd10e-116">string</span></span> |  <span data-ttu-id="cd10e-117">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd10e-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="cd10e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd10e-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
