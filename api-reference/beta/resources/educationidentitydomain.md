---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807751"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="eabe9-104">Тип ресурса educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="eabe9-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="eabe9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eabe9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eabe9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eabe9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eabe9-107">Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="eabe9-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="eabe9-108">Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eabe9-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="eabe9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eabe9-109">Properties</span></span>

| <span data-ttu-id="eabe9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eabe9-110">Property</span></span> | <span data-ttu-id="eabe9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eabe9-111">Type</span></span> | <span data-ttu-id="eabe9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eabe9-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="eabe9-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="eabe9-113">**appliesTo**</span></span> | <span data-ttu-id="eabe9-114">string</span><span class="sxs-lookup"><span data-stu-id="eabe9-114">string</span></span> |  <span data-ttu-id="eabe9-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="eabe9-115">The user role type to assign to license.</span></span> <span data-ttu-id="eabe9-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="eabe9-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="eabe9-117">**name**</span><span class="sxs-lookup"><span data-stu-id="eabe9-117">**name**</span></span> | <span data-ttu-id="eabe9-118">строка</span><span class="sxs-lookup"><span data-stu-id="eabe9-118">string</span></span> |  <span data-ttu-id="eabe9-119">Представляет учетную запись пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="eabe9-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="eabe9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eabe9-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
