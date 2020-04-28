---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a21d4d3005be8a776ae8bb9f9e3c1027be48de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501929"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="4975e-104">Тип ресурса Едукатионидентитидомаин</span><span class="sxs-lookup"><span data-stu-id="4975e-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="4975e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4975e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4975e-106">Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="4975e-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="4975e-107">Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4975e-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="4975e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4975e-108">Properties</span></span>

| <span data-ttu-id="4975e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4975e-109">Property</span></span> | <span data-ttu-id="4975e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4975e-110">Type</span></span> | <span data-ttu-id="4975e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4975e-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4975e-112">**Тег**</span><span class="sxs-lookup"><span data-stu-id="4975e-112">**appliesTo**</span></span> | <span data-ttu-id="4975e-113">string</span><span class="sxs-lookup"><span data-stu-id="4975e-113">string</span></span> |  <span data-ttu-id="4975e-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="4975e-114">The user role type to assign to the license.</span></span> <span data-ttu-id="4975e-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="4975e-115">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="4975e-116">**name**</span><span class="sxs-lookup"><span data-stu-id="4975e-116">**name**</span></span> | <span data-ttu-id="4975e-117">string</span><span class="sxs-lookup"><span data-stu-id="4975e-117">string</span></span> |  <span data-ttu-id="4975e-118">Представляет домен для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="4975e-118">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="4975e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4975e-119">JSON representation</span></span>
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
