---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7c26ef1447272b88c59ec6992e41ae051439645e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095396"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="67b60-105">Тип ресурса Едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="67b60-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b60-106">Определяет параметры для согласованных удостоверений профиля данных учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="67b60-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="67b60-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="67b60-107">These identities include students and teachers.</span></span> <span data-ttu-id="67b60-108">На основе этих параметров пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="67b60-108">Based on these settings, the users will be updated in the directory.</span></span>

> [!NOTE]
> <span data-ttu-id="67b60-109">При выборе этого ресурса пользователи не создаются.</span><span class="sxs-lookup"><span data-stu-id="67b60-109">No Users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="67b60-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="67b60-110">Properties</span></span>

| <span data-ttu-id="67b60-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="67b60-111">Property</span></span>        | <span data-ttu-id="67b60-112">Тип</span><span class="sxs-lookup"><span data-stu-id="67b60-112">Type</span></span>                                                                                               | <span data-ttu-id="67b60-113">Описание</span><span class="sxs-lookup"><span data-stu-id="67b60-113">Description</span></span>                                                                                      |
| :-------------- | :------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="67b60-114">матчингоптионс</span><span class="sxs-lookup"><span data-stu-id="67b60-114">matchingOptions</span></span> | <span data-ttu-id="67b60-115">Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="67b60-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="67b60-116">Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление.</span><span class="sxs-lookup"><span data-stu-id="67b60-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67b60-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67b60-117">JSON representation</span></span>

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
      "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```


