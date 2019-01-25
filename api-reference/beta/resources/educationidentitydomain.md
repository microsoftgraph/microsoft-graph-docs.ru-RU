---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528181"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="02e42-104">Тип ресурса educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="02e42-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02e42-105">Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="02e42-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="02e42-106">Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02e42-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="02e42-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="02e42-107">Properties</span></span>

| <span data-ttu-id="02e42-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="02e42-108">Property</span></span> | <span data-ttu-id="02e42-109">Тип</span><span class="sxs-lookup"><span data-stu-id="02e42-109">Type</span></span> | <span data-ttu-id="02e42-110">Описание</span><span class="sxs-lookup"><span data-stu-id="02e42-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="02e42-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="02e42-111">**appliesTo**</span></span> | <span data-ttu-id="02e42-112">string</span><span class="sxs-lookup"><span data-stu-id="02e42-112">string</span></span> |  <span data-ttu-id="02e42-113">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="02e42-113">The user role type to assign to license.</span></span> <span data-ttu-id="02e42-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="02e42-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="02e42-115">**name**</span><span class="sxs-lookup"><span data-stu-id="02e42-115">**name**</span></span> | <span data-ttu-id="02e42-116">строка</span><span class="sxs-lookup"><span data-stu-id="02e42-116">string</span></span> |  <span data-ttu-id="02e42-117">Представляет учетную запись пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="02e42-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="02e42-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02e42-118">JSON representation</span></span>
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
