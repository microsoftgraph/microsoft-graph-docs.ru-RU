---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507121"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="aa1df-105">Тип ресурса Едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aa1df-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa1df-106">Определяет параметры для согласованных удостоверений профиля данных учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="aa1df-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="aa1df-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="aa1df-107">These identities include students and teachers.</span></span> <span data-ttu-id="aa1df-108">На основе этих параметров пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="aa1df-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="aa1df-109">**Примечание:** При выборе этого ресурса пользователи не создаются.</span><span class="sxs-lookup"><span data-stu-id="aa1df-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="aa1df-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa1df-110">Properties</span></span>

| <span data-ttu-id="aa1df-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa1df-111">Property</span></span> | <span data-ttu-id="aa1df-112">Тип</span><span class="sxs-lookup"><span data-stu-id="aa1df-112">Type</span></span> | <span data-ttu-id="aa1df-113">Описание</span><span class="sxs-lookup"><span data-stu-id="aa1df-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="aa1df-114">**Матчингоптионс**</span><span class="sxs-lookup"><span data-stu-id="aa1df-114">**matchingOptions**</span></span> | <span data-ttu-id="aa1df-115">Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="aa1df-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="aa1df-116">Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление.</span><span class="sxs-lookup"><span data-stu-id="aa1df-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa1df-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa1df-117">JSON representation</span></span>
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
