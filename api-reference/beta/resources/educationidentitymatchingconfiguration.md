---
title: Тип ресурса educationIdentityMatchingConfiguration
description: Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ded27e432219a247bf9c03c21f8ebd0054183eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411332"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="6addd-105">Тип ресурса educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="6addd-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="6addd-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6addd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6addd-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6addd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6addd-108">Задает параметры для сопоставления школа данных профиля удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6addd-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="6addd-109">Эти удостоверения включают студентов и преподавателей.</span><span class="sxs-lookup"><span data-stu-id="6addd-109">These identities include students and teachers.</span></span> <span data-ttu-id="6addd-110">На основе этих параметров, пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6addd-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="6addd-111">**Примечание:** Пользователи не создаются при выборе этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="6addd-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="6addd-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6addd-112">Properties</span></span>

| <span data-ttu-id="6addd-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6addd-113">Property</span></span> | <span data-ttu-id="6addd-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6addd-114">Type</span></span> | <span data-ttu-id="6addd-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6addd-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6addd-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="6addd-116">**matchingOptions**</span></span> | <span data-ttu-id="6addd-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6addd-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="6addd-118">Сопоставление учетной записи пользователя и параметры, используемые для уникальной идентификации пользователя для обновления.</span><span class="sxs-lookup"><span data-stu-id="6addd-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6addd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6addd-119">JSON representation</span></span>
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
