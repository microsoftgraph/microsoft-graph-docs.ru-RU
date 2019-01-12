---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982031"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="35235-104">Тип ресурса educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="35235-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="35235-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35235-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35235-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35235-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35235-107">Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="35235-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="35235-108">Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35235-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="35235-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="35235-109">Properties</span></span>

| <span data-ttu-id="35235-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="35235-110">Property</span></span> | <span data-ttu-id="35235-111">Тип</span><span class="sxs-lookup"><span data-stu-id="35235-111">Type</span></span> | <span data-ttu-id="35235-112">Описание</span><span class="sxs-lookup"><span data-stu-id="35235-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="35235-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="35235-113">**appliesTo**</span></span> | <span data-ttu-id="35235-114">string</span><span class="sxs-lookup"><span data-stu-id="35235-114">string</span></span> |  <span data-ttu-id="35235-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="35235-115">The user role type to assign to license.</span></span> <span data-ttu-id="35235-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="35235-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="35235-117">**name**</span><span class="sxs-lookup"><span data-stu-id="35235-117">**name**</span></span> | <span data-ttu-id="35235-118">строка</span><span class="sxs-lookup"><span data-stu-id="35235-118">string</span></span> |  <span data-ttu-id="35235-119">Представляет учетную запись пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="35235-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="35235-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35235-120">JSON representation</span></span>
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
