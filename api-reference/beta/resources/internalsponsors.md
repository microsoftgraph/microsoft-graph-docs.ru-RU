---
title: тип internalSponsors сложный
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c53bbeacde51afc88f5c0b4b5c13bc4f68b430
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760899"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="7e728-103">тип internalSponsors сложный</span><span class="sxs-lookup"><span data-stu-id="7e728-103">internalSponsors complex type</span></span>

<span data-ttu-id="7e728-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e728-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e728-105">Используется на этапе утверждения политики [назначения пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7e728-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="7e728-106">Это подтип [userSet,](userset.md)в котором значение указывает, что внутренними спонсорами, запрашивающие подключенную организацию пользователя, должны `@odata.type` `#microsoft.graph.internalSponsors` быть утверждены.</span><span class="sxs-lookup"><span data-stu-id="7e728-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="7e728-107">Этот одобрение применимо только к запросам пользователей, которые являются частью связанной организации.</span><span class="sxs-lookup"><span data-stu-id="7e728-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="7e728-108">При создании этапа утверждения политики назначения пакетов доступа с помощью внутреннихSponsors также включаем другого участника, например одного пользователя или члена группы, в случае, если подключенная организация не имеет внутреннего спонсора.</span><span class="sxs-lookup"><span data-stu-id="7e728-108">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="7e728-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e728-109">Properties</span></span>

| <span data-ttu-id="7e728-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e728-110">Property</span></span>                     | <span data-ttu-id="7e728-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7e728-111">Type</span></span>                      | <span data-ttu-id="7e728-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7e728-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="7e728-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="7e728-113">isBackup</span></span> | <span data-ttu-id="7e728-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e728-114">Boolean</span></span> | <span data-ttu-id="7e728-115">Указывает, является ли автор резервного копирования автором резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="7e728-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e728-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e728-116">JSON representation</span></span>

<span data-ttu-id="7e728-117">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="7e728-117">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


