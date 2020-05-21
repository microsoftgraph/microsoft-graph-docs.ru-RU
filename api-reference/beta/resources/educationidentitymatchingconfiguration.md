---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fd42bc30a1cc1cee34685bc0f33815f3a00d0120
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336029"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="87429-105">Тип ресурса Едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="87429-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87429-106">Определяет параметры для согласованных удостоверений профиля данных учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="87429-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="87429-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="87429-107">These identities include students and teachers.</span></span> <span data-ttu-id="87429-108">На основе этих параметров пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="87429-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="87429-109">**Примечание:** При выборе этого ресурса пользователи не создаются.</span><span class="sxs-lookup"><span data-stu-id="87429-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="87429-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="87429-110">Properties</span></span>

| <span data-ttu-id="87429-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="87429-111">Property</span></span> | <span data-ttu-id="87429-112">Тип</span><span class="sxs-lookup"><span data-stu-id="87429-112">Type</span></span> | <span data-ttu-id="87429-113">Описание</span><span class="sxs-lookup"><span data-stu-id="87429-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="87429-114">**матчингоптионс**</span><span class="sxs-lookup"><span data-stu-id="87429-114">**matchingOptions**</span></span> | <span data-ttu-id="87429-115">Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="87429-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="87429-116">Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление.</span><span class="sxs-lookup"><span data-stu-id="87429-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87429-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87429-117">JSON representation</span></span>
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
