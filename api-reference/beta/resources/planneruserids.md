---
title: Тип ресурса Планнерусеридс
description: Ресурс **планнерусеридс** представляет список идентификаторов пользователей, к которым предоставлен общий доступ к плану. Это открытый тип. Если вы используете группы Office 365, используйте API групп для управления членством в группах, чтобы поделиться планом группы. Вы также можете добавить существующих членов группы в эту коллекцию, несмотря на то, что они не требуются для доступа к плану, принадлежащему группе.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 83717714d58cd0c442b42c23c9aa361bcd3b2261
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344391"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="72d58-106">Тип ресурса Планнерусеридс</span><span class="sxs-lookup"><span data-stu-id="72d58-106">plannerUserIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d58-107">Ресурс **планнерусеридс** представляет список идентификаторов пользователей, к которым предоставлен [](plannerplan.md) общий доступ к плану.</span><span class="sxs-lookup"><span data-stu-id="72d58-107">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with.</span></span> <span data-ttu-id="72d58-108">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="72d58-108">This is an Open Type.</span></span> <span data-ttu-id="72d58-109">Если вы используете группы Office 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="72d58-109">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="72d58-110">Вы также можете добавить существующих членов группы в эту коллекцию, несмотря на то, что они не требуются для доступа к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="72d58-110">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="72d58-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="72d58-111">Properties</span></span>
<span data-ttu-id="72d58-112">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="72d58-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="72d58-113">В этом случае клиент должен предоставить идентификаторы пользователей как свойства с `true` логическими значениями.</span><span class="sxs-lookup"><span data-stu-id="72d58-113">In this case, the client should provide user ids as properties with their values being the `true` boolean.</span></span> <span data-ttu-id="72d58-114">Если к идентификаторам пользователей больше не предоставляется доступ, свойства автоматически удаляются путем присвоения их значений `false` логическому значению.</span><span class="sxs-lookup"><span data-stu-id="72d58-114">When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="72d58-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72d58-115">JSON representation</span></span>

<span data-ttu-id="72d58-116">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="72d58-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="72d58-117">Примеры</span><span class="sxs-lookup"><span data-stu-id="72d58-117">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
