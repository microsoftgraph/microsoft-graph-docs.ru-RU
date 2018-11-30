---
title: Тип ресурса plannerUserIds
description: Ресурс **plannerUserIds** представляет список идентификаторов пользователей, которым предоставлен доступ к плану. Это открытый тип. Если вы используете функцию "Группы Office 365", то для предоставления доступа к плану группы применяйте API для групп (чтобы управлять членством в группах). Вы также можете добавить существующих участников группы в эту коллекцию, хотя им необязательно иметь доступ к плану, принадлежащему группе.
ms.openlocfilehash: 4bbe0b5c28d838605975a2cdc3c28a529f3725f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082231"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="a2405-106">Тип ресурса plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a2405-106">plannerUserIds resource type</span></span>

> <span data-ttu-id="a2405-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2405-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2405-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2405-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2405-p103">Ресурс **plannerUserIds** представляет список идентификаторов пользователей, которым предоставлен доступ к [плану](plannerplan.md). Это открытый тип. Если вы используете функцию "Группы Office 365", то для предоставления доступа к плану [группы](group.md) применяйте API для групп (чтобы управлять членством в группах). Вы также можете добавить существующих участников группы в эту коллекцию, хотя им необязательно иметь доступ к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="a2405-p103">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with. This is an Open Type. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="a2405-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2405-113">Properties</span></span>
<span data-ttu-id="a2405-p104">Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы пользователей в качестве свойств, причем они должны иметь значение `true` (логическое). Если больше не нужно предоставлять доступ для идентификаторов пользователей, задайте для свойств значение `false` (логическое), и свойства будут автоматически удалены.</span><span class="sxs-lookup"><span data-stu-id="a2405-p104">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2405-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2405-117">JSON representation</span></span>

<span data-ttu-id="a2405-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2405-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="a2405-119">Пример:</span><span class="sxs-lookup"><span data-stu-id="a2405-119">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->