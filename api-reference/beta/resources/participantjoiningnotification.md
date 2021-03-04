---
title: тип ресурса participantJoiningNotification
description: Содержит сведения о присоединении участника, основанного на политике, к вызову.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a0067f5632e34a30da7f6f4ec2e8df70995fa88
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447519"
---
# <a name="participantjoiningnotification-resource-type"></a><span data-ttu-id="5fe36-103">тип ресурса participantJoiningNotification</span><span class="sxs-lookup"><span data-stu-id="5fe36-103">participantJoiningNotification resource type</span></span>

<span data-ttu-id="5fe36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fe36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fe36-105">Содержит сведения о присоединении участника, основанного на политике, к вызову.</span><span class="sxs-lookup"><span data-stu-id="5fe36-105">Contains details about the policy-based participant joining a call.</span></span>

<span data-ttu-id="5fe36-106">В [сценарии](/microsoftteams/teams-recording-policy)записи на основе политики перед тем, как участник политики присоединяется к вызову, боту, связанному с политикой, которая имеет доступную емкость для обработки нового участника, будет `participantJoiningNotification` отправлено.</span><span class="sxs-lookup"><span data-stu-id="5fe36-106">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under the policy joins a call, a `participantJoiningNotification` will be sent to the bot associated with the policy that has available capacity to handle the new participant.</span></span>

<span data-ttu-id="5fe36-107">[УчастникJoiningResponse в](participantjoiningResponse.md) ответной нагрузке ожидается от бота.</span><span class="sxs-lookup"><span data-stu-id="5fe36-107">A [participantJoiningResponse](participantjoiningResponse.md) in the response payload is expected from the bot.</span></span>

## <a name="properties"></a><span data-ttu-id="5fe36-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fe36-108">Properties</span></span>
| <span data-ttu-id="5fe36-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fe36-109">Property</span></span>       | <span data-ttu-id="5fe36-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5fe36-110">Type</span></span>            | <span data-ttu-id="5fe36-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe36-111">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="5fe36-112">call</span><span class="sxs-lookup"><span data-stu-id="5fe36-112">call</span></span>           | [<span data-ttu-id="5fe36-113">call</span><span class="sxs-lookup"><span data-stu-id="5fe36-113">call</span></span>](call.md) | <span data-ttu-id="5fe36-114">Объект вызова, содержащий сведения о событии присоединения участника.</span><span class="sxs-lookup"><span data-stu-id="5fe36-114">The call object that contains details about the participant joining event.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5fe36-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fe36-115">JSON representation</span></span>

<span data-ttu-id="5fe36-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe36-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

