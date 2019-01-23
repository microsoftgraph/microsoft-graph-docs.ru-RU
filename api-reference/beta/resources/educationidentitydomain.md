---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4eb9e5b58f62a23dbe1b450c2ec6b9d2f94970ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395652"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="74aa8-104">Тип ресурса educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="74aa8-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="74aa8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74aa8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74aa8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74aa8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74aa8-107">Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="74aa8-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="74aa8-108">Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74aa8-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="74aa8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="74aa8-109">Properties</span></span>

| <span data-ttu-id="74aa8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="74aa8-110">Property</span></span> | <span data-ttu-id="74aa8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="74aa8-111">Type</span></span> | <span data-ttu-id="74aa8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74aa8-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="74aa8-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="74aa8-113">**appliesTo**</span></span> | <span data-ttu-id="74aa8-114">string</span><span class="sxs-lookup"><span data-stu-id="74aa8-114">string</span></span> |  <span data-ttu-id="74aa8-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="74aa8-115">The user role type to assign to license.</span></span> <span data-ttu-id="74aa8-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="74aa8-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="74aa8-117">**name**</span><span class="sxs-lookup"><span data-stu-id="74aa8-117">**name**</span></span> | <span data-ttu-id="74aa8-118">строка</span><span class="sxs-lookup"><span data-stu-id="74aa8-118">string</span></span> |  <span data-ttu-id="74aa8-119">Представляет учетную запись пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="74aa8-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="74aa8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74aa8-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
