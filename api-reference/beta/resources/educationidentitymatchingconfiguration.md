---
title: Тип ресурса educationIdentityMatchingConfiguration
description: Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.
ms.openlocfilehash: b189735340c121a56c48ae21518989cf8e1634f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081952"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="07332-105">Тип ресурса educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="07332-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="07332-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07332-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07332-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07332-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07332-108">Задает параметры для сопоставления школа данных профиля удостоверения.</span><span class="sxs-lookup"><span data-stu-id="07332-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="07332-109">Эти удостоверения включают студентов и преподавателей.</span><span class="sxs-lookup"><span data-stu-id="07332-109">These identities include students and teachers.</span></span> <span data-ttu-id="07332-110">На основе этих параметров, пользователи будут обновлены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="07332-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="07332-111">**Примечание:** Пользователи не создаются при выборе этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="07332-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="07332-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="07332-112">Properties</span></span>

| <span data-ttu-id="07332-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="07332-113">Property</span></span> | <span data-ttu-id="07332-114">Тип</span><span class="sxs-lookup"><span data-stu-id="07332-114">Type</span></span> | <span data-ttu-id="07332-115">Description</span><span class="sxs-lookup"><span data-stu-id="07332-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="07332-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="07332-116">**matchingOptions**</span></span> | <span data-ttu-id="07332-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="07332-117">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="07332-118">Сопоставление учетной записи пользователя и параметры, используемые для уникальной идентификации пользователя для обновления.</span><span class="sxs-lookup"><span data-stu-id="07332-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="07332-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07332-119">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
