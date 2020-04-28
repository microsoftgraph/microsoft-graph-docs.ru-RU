---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6805fabd857e4e906fa095c372632edbcc27fa28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006390"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="454ac-105">Тип ресурса Едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="454ac-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="454ac-106">Определяет параметры для согласованных удостоверений профиля данных учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="454ac-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="454ac-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="454ac-107">These identities include students and teachers.</span></span> <span data-ttu-id="454ac-108">На основе этих параметров пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="454ac-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="454ac-109">**Примечание:** При выборе этого ресурса пользователи не создаются.</span><span class="sxs-lookup"><span data-stu-id="454ac-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="454ac-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="454ac-110">Properties</span></span>

| <span data-ttu-id="454ac-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="454ac-111">Property</span></span> | <span data-ttu-id="454ac-112">Тип</span><span class="sxs-lookup"><span data-stu-id="454ac-112">Type</span></span> | <span data-ttu-id="454ac-113">Описание</span><span class="sxs-lookup"><span data-stu-id="454ac-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="454ac-114">**матчингоптионс**</span><span class="sxs-lookup"><span data-stu-id="454ac-114">**matchingOptions**</span></span> | <span data-ttu-id="454ac-115">Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="454ac-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="454ac-116">Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление.</span><span class="sxs-lookup"><span data-stu-id="454ac-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="454ac-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="454ac-117">JSON representation</span></span>
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
