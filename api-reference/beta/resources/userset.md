---
title: Сложный тип userSet
description: Абстрактный базовый тип для типов, используемых в параметрах проверки запросов, утверждений и назначений политики назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 541bce7c65eaa9b284e9da5b520913b1be4ca8a3
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777727"
---
# <a name="userset-complex-type"></a><span data-ttu-id="05aa6-103">Сложный тип userSet</span><span class="sxs-lookup"><span data-stu-id="05aa6-103">userSet complex type</span></span>

<span data-ttu-id="05aa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05aa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05aa6-105">Используется в параметрах проверки запроса, утверждения и назначения политики [назначения пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="05aa6-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="05aa6-106">Абстрактный базовый тип для типов [singleUser,](singleuser.md)[groupMembers,](groupmembers.md) [connectedOrganizationMembers,](connectedorganizationmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md)и [externalSponsors.](externalsponsors.md)</span><span class="sxs-lookup"><span data-stu-id="05aa6-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="05aa6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="05aa6-107">Properties</span></span>

| <span data-ttu-id="05aa6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="05aa6-108">Property</span></span>                     | <span data-ttu-id="05aa6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="05aa6-109">Type</span></span>                      | <span data-ttu-id="05aa6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05aa6-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="05aa6-111">isBackup</span><span class="sxs-lookup"><span data-stu-id="05aa6-111">isBackup</span></span> | <span data-ttu-id="05aa6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="05aa6-112">Boolean</span></span> | <span data-ttu-id="05aa6-113">Для пользователя на стадии утверждения это свойство указывает, является ли пользователь резервным утверждением резервной копии.</span><span class="sxs-lookup"><span data-stu-id="05aa6-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05aa6-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05aa6-114">JSON representation</span></span>

<span data-ttu-id="05aa6-115">Ниже приводится представление userSet в JSON.</span><span class="sxs-lookup"><span data-stu-id="05aa6-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="05aa6-116">Обратите внимание, что userSet — это абстрактный базовый класс, поэтому он не будет отправлен или получен.</span><span class="sxs-lookup"><span data-stu-id="05aa6-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="05aa6-117">Вместо этого будет использоваться один из `@odata.type` `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` , `#microsoft.graph.connectedOrganizationMembers` ", `#microsoft.graph.requestorManager` " `#microsoft.graph.internalSponsors` `#microsoft.graph.externalSponsors` или " .</span><span class="sxs-lookup"><span data-stu-id="05aa6-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


