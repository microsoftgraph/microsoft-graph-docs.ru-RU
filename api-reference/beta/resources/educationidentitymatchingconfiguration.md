---
title: Тип ресурса educationIdentityMatchingConfiguration
description: Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520314"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="15726-105">Тип ресурса educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="15726-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15726-106">Задает параметры для сопоставления школа данных профиля удостоверения.</span><span class="sxs-lookup"><span data-stu-id="15726-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="15726-107">Эти удостоверения включают студентов и преподавателей.</span><span class="sxs-lookup"><span data-stu-id="15726-107">These identities include students and teachers.</span></span> <span data-ttu-id="15726-108">На основе этих параметров, пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="15726-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="15726-109">**Примечание:** Пользователи не создаются при выборе этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="15726-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="15726-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="15726-110">Properties</span></span>

| <span data-ttu-id="15726-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="15726-111">Property</span></span> | <span data-ttu-id="15726-112">Тип</span><span class="sxs-lookup"><span data-stu-id="15726-112">Type</span></span> | <span data-ttu-id="15726-113">Описание</span><span class="sxs-lookup"><span data-stu-id="15726-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="15726-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="15726-114">**matchingOptions**</span></span> | <span data-ttu-id="15726-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15726-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="15726-116">Сопоставление учетной записи пользователя и параметры, используемые для уникальной идентификации пользователя для обновления.</span><span class="sxs-lookup"><span data-stu-id="15726-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15726-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15726-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
