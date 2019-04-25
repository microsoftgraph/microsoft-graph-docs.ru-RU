---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543118"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="bc91e-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="bc91e-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc91e-105">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc91e-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="bc91e-106">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bc91e-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="bc91e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc91e-107">Properties</span></span>

| <span data-ttu-id="bc91e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc91e-108">Property</span></span> | <span data-ttu-id="bc91e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc91e-109">Type</span></span> | <span data-ttu-id="bc91e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc91e-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bc91e-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="bc91e-111">**appliesTo**</span></span> | <span data-ttu-id="bc91e-112">string</span><span class="sxs-lookup"><span data-stu-id="bc91e-112">string</span></span> |  <span data-ttu-id="bc91e-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="bc91e-113">The user role type to assign to license.</span></span> <span data-ttu-id="bc91e-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="bc91e-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="bc91e-115">**name**</span><span class="sxs-lookup"><span data-stu-id="bc91e-115">**name**</span></span> | <span data-ttu-id="bc91e-116">string</span><span class="sxs-lookup"><span data-stu-id="bc91e-116">string</span></span> |  <span data-ttu-id="bc91e-117">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc91e-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="bc91e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc91e-118">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
