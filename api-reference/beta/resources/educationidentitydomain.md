---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5cf7444c51b34ae4a8eacf9c99fdfd085dbec896
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334270"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="96267-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="96267-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96267-105">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="96267-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="96267-106">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96267-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="96267-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="96267-107">Properties</span></span>

| <span data-ttu-id="96267-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="96267-108">Property</span></span> | <span data-ttu-id="96267-109">Тип</span><span class="sxs-lookup"><span data-stu-id="96267-109">Type</span></span> | <span data-ttu-id="96267-110">Описание</span><span class="sxs-lookup"><span data-stu-id="96267-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="96267-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="96267-111">**appliesTo**</span></span> | <span data-ttu-id="96267-112">string</span><span class="sxs-lookup"><span data-stu-id="96267-112">string</span></span> |  <span data-ttu-id="96267-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="96267-113">The user role type to assign to license.</span></span> <span data-ttu-id="96267-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="96267-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="96267-115">**name**</span><span class="sxs-lookup"><span data-stu-id="96267-115">**name**</span></span> | <span data-ttu-id="96267-116">string</span><span class="sxs-lookup"><span data-stu-id="96267-116">string</span></span> |  <span data-ttu-id="96267-117">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="96267-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="96267-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96267-118">JSON representation</span></span>
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
