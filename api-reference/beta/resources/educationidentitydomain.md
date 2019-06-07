---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 628fbdea770c685eca0194fb95a314e2e542d2fc
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750159"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="947e0-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="947e0-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="947e0-105">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="947e0-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="947e0-106">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="947e0-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="947e0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="947e0-107">Properties</span></span>

| <span data-ttu-id="947e0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="947e0-108">Property</span></span> | <span data-ttu-id="947e0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="947e0-109">Type</span></span> | <span data-ttu-id="947e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="947e0-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="947e0-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="947e0-111">**appliesTo**</span></span> | <span data-ttu-id="947e0-112">string</span><span class="sxs-lookup"><span data-stu-id="947e0-112">string</span></span> |  <span data-ttu-id="947e0-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="947e0-113">The user role type to assign to the license.</span></span> <span data-ttu-id="947e0-114">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="947e0-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="947e0-115">**name**</span><span class="sxs-lookup"><span data-stu-id="947e0-115">**name**</span></span> | <span data-ttu-id="947e0-116">string</span><span class="sxs-lookup"><span data-stu-id="947e0-116">string</span></span> |  <span data-ttu-id="947e0-117">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="947e0-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="947e0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="947e0-118">JSON representation</span></span>
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
