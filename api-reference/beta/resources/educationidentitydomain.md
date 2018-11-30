---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080017"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="6537e-104">Тип ресурса educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="6537e-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="6537e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6537e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6537e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6537e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6537e-107">Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="6537e-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="6537e-108">Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6537e-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="6537e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6537e-109">Properties</span></span>

| <span data-ttu-id="6537e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6537e-110">Property</span></span> | <span data-ttu-id="6537e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6537e-111">Type</span></span> | <span data-ttu-id="6537e-112">Description</span><span class="sxs-lookup"><span data-stu-id="6537e-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6537e-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="6537e-113">**appliesTo**</span></span> | <span data-ttu-id="6537e-114">string</span><span class="sxs-lookup"><span data-stu-id="6537e-114">string</span></span> |  <span data-ttu-id="6537e-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="6537e-115">The user role type to assign to license.</span></span> <span data-ttu-id="6537e-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="6537e-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="6537e-117">**name**</span><span class="sxs-lookup"><span data-stu-id="6537e-117">**name**</span></span> | <span data-ttu-id="6537e-118">строка</span><span class="sxs-lookup"><span data-stu-id="6537e-118">string</span></span> |  <span data-ttu-id="6537e-119">Представляет учетную запись пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="6537e-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="6537e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6537e-120">JSON representation</span></span>
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
