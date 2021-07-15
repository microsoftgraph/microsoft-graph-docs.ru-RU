---
title: тип ресурса participantLeftNotification
description: Содержит сведения о участнике, основанном на политике, который покинул вызов.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ee2526ceef6aaf377003f6e802093ec103059c06
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430854"
---
# <a name="participantleftnotification-resource-type"></a><span data-ttu-id="c4d24-103">тип ресурса participantLeftNotification</span><span class="sxs-lookup"><span data-stu-id="c4d24-103">participantLeftNotification resource type</span></span>

<span data-ttu-id="c4d24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4d24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4d24-105">Содержит сведения о участнике, основанном на политике, который покинул вызов.</span><span class="sxs-lookup"><span data-stu-id="c4d24-105">Contains details about the policy-based participant who has left the call.</span></span>

<span data-ttu-id="c4d24-106">В [сценарии](/microsoftteams/teams-recording-policy) записи на основе политики, когда участник, управляемый вызовом бота, покинул собрание, боту будет отправлено уведомление бота с сведениями о событии, оставленного `participantLeftNotification` участником.</span><span class="sxs-lookup"><span data-stu-id="c4d24-106">Under the [Policy-based recording](/microsoftteams/teams-recording-policy) scenario, when a participant who is managed by the bot call has left the meeting, a `participantLeftNotification` will be sent to the bot to notify the bot with details of the participant left event.</span></span>

## <a name="properties"></a><span data-ttu-id="c4d24-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4d24-107">Properties</span></span>
| <span data-ttu-id="c4d24-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4d24-108">Property</span></span>       | <span data-ttu-id="c4d24-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c4d24-109">Type</span></span>            | <span data-ttu-id="c4d24-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4d24-110">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="c4d24-111">call</span><span class="sxs-lookup"><span data-stu-id="c4d24-111">call</span></span>           | [<span data-ttu-id="c4d24-112">call</span><span class="sxs-lookup"><span data-stu-id="c4d24-112">call</span></span>](call.md) | <span data-ttu-id="c4d24-113">Объект вызова, содержащий сведения о событии присоединения участника.</span><span class="sxs-lookup"><span data-stu-id="c4d24-113">The call object that contains details about the participant joining event.</span></span> |
| <span data-ttu-id="c4d24-114">participantId</span><span class="sxs-lookup"><span data-stu-id="c4d24-114">participantId</span></span>  | <span data-ttu-id="c4d24-115">String</span><span class="sxs-lookup"><span data-stu-id="c4d24-115">String</span></span>          | <span data-ttu-id="c4d24-116">ID участника в соответствии с политикой, которая покинула собрание.</span><span class="sxs-lookup"><span data-stu-id="c4d24-116">ID of the participant under the policy who has left the meeting.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="c4d24-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4d24-117">JSON representation</span></span>

<span data-ttu-id="c4d24-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4d24-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
