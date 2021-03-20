---
title: тип ресурса broadcastMeetingSettings
description: Параметры, связанные с событием в прямом эфире
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: def9276d97ddbe1fd812083cc17e547ae7ce53c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953763"
---
# <a name="broadcastmeetingsettings-resource-type"></a><span data-ttu-id="ae44e-103">тип ресурса broadcastMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="ae44e-103">broadcastMeetingSettings resource type</span></span>

<span data-ttu-id="ae44e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae44e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae44e-105">Параметры, связанные с живым событием.</span><span class="sxs-lookup"><span data-stu-id="ae44e-105">Settings related to a live event.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ae44e-106">Этот API не проверяет параметры событий в прямом эфире, управляемые [политикой.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="ae44e-106">This API does not validate live event settings that are managed by [policy](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).</span></span>
> <span data-ttu-id="ae44e-107">Например, если администратор задает политику событий в прямом эфире с помощью, пользователям будет запрещено устанавливать разрешения на живые события в клиенте Teams, но он сможет создать живое событие с помощью `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` Microsoft Graph,  `everyone` установив разрешенное разрешение на .</span><span class="sxs-lookup"><span data-stu-id="ae44e-107">For example, if an admin sets a live event policy using `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany`, users will be prevented from setting live event permissions to `public` in their Teams client, but will be able to create a live event via Microsoft Graph by setting **allowedAudience** to `everyone`.</span></span> 

## <a name="properties"></a><span data-ttu-id="ae44e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae44e-108">Properties</span></span>

| <span data-ttu-id="ae44e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae44e-109">Property</span></span>                   | <span data-ttu-id="ae44e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ae44e-110">Type</span></span>                     | <span data-ttu-id="ae44e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ae44e-111">Description</span></span>                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| <span data-ttu-id="ae44e-112">allowedAudience</span><span class="sxs-lookup"><span data-stu-id="ae44e-112">allowedAudience</span></span>            | [<span data-ttu-id="ae44e-113">broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="ae44e-113">broadcastMeetingAudience</span></span>](#broadcastmeetingaudience-values) | <span data-ttu-id="ae44e-114">Определяет, кто может присоединиться к событию в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-114">Defines who can join the live event.</span></span> <span data-ttu-id="ae44e-115">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ae44e-115">Possible values are listed in the following table.</span></span> |
| <span data-ttu-id="ae44e-116">isRecordingEnabled</span><span class="sxs-lookup"><span data-stu-id="ae44e-116">isRecordingEnabled</span></span>         | <span data-ttu-id="ae44e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae44e-117">Boolean</span></span>                  | <span data-ttu-id="ae44e-118">Указывает, включена ли запись для этого события в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-118">Indicates whether recording is enabled for this live event.</span></span> <span data-ttu-id="ae44e-119">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="ae44e-119">Default value is `false`.</span></span>          |
| <span data-ttu-id="ae44e-120">isAttendeeReportEnabled</span><span class="sxs-lookup"><span data-stu-id="ae44e-120">isAttendeeReportEnabled</span></span>    | <span data-ttu-id="ae44e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae44e-121">Boolean</span></span>                  | <span data-ttu-id="ae44e-122">Указывает, включен ли отчет участника для этого события в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-122">Indicates whether attendee report is enabled for this live event.</span></span> <span data-ttu-id="ae44e-123">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="ae44e-123">Default value is `false`.</span></span>    |
| <span data-ttu-id="ae44e-124">isQuestionAndAnswerEnabled</span><span class="sxs-lookup"><span data-stu-id="ae44e-124">isQuestionAndAnswerEnabled</span></span> | <span data-ttu-id="ae44e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae44e-125">Boolean</span></span>                  | <span data-ttu-id="ae44e-126">Указывает, включен ли Q&A для этого события в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-126">Indicates whether Q&A is enabled for this live event.</span></span> <span data-ttu-id="ae44e-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="ae44e-127">Default value is `false`.</span></span>                |
| <span data-ttu-id="ae44e-128">isVideoOnDemandEnabled</span><span class="sxs-lookup"><span data-stu-id="ae44e-128">isVideoOnDemandEnabled</span></span>     | <span data-ttu-id="ae44e-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae44e-129">Boolean</span></span>                  | <span data-ttu-id="ae44e-130">Указывает, включено ли видео по запросу для этого события в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-130">Indicates whether video on demand is enabled for this live event.</span></span> <span data-ttu-id="ae44e-131">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="ae44e-131">Default value is `false`.</span></span>    |

### <a name="broadcastmeetingaudience-values"></a><span data-ttu-id="ae44e-132">значения broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="ae44e-132">broadcastMeetingAudience values</span></span>

| <span data-ttu-id="ae44e-133">Значение</span><span class="sxs-lookup"><span data-stu-id="ae44e-133">Value</span></span>              | <span data-ttu-id="ae44e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ae44e-134">Description</span></span>                                                       |
| ------------------ | ----------------------------------------------------------------- |
| <span data-ttu-id="ae44e-135">все</span><span class="sxs-lookup"><span data-stu-id="ae44e-135">everyone</span></span>           | <span data-ttu-id="ae44e-136">Событие в прямом эфире будет открыто для всех.</span><span class="sxs-lookup"><span data-stu-id="ae44e-136">The live event will be open to anyone.</span></span> <span data-ttu-id="ae44e-137">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ae44e-137">This is the default value.</span></span> |
| <span data-ttu-id="ae44e-138">organization;</span><span class="sxs-lookup"><span data-stu-id="ae44e-138">organization</span></span>       | <span data-ttu-id="ae44e-139">Все в вашей организации могут присоединиться к событию в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-139">Everyone in your org can join the live event.</span></span>                     |
| <span data-ttu-id="ae44e-140">roleIsAttendee</span><span class="sxs-lookup"><span data-stu-id="ae44e-140">roleIsAttendee</span></span>     | <span data-ttu-id="ae44e-141">Только указанные люди могут присоединиться к событию в прямом эфире.</span><span class="sxs-lookup"><span data-stu-id="ae44e-141">Only the specified people can join the live event.</span></span>                |
| <span data-ttu-id="ae44e-142">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="ae44e-142">unknownFutureValue</span></span> | <span data-ttu-id="ae44e-143">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="ae44e-143">Unknown future value.</span></span>                                             |

## <a name="json-representation"></a><span data-ttu-id="ae44e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae44e-144">JSON representation</span></span>

<span data-ttu-id="ae44e-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae44e-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
