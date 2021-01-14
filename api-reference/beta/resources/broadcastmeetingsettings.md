---
title: Тип ресурса broadcastMeetingSettings
description: Параметры, связанные с трансляцией
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42ac666817b6f259dd888e479939216fc3e39c6c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866254"
---
# <a name="broadcastmeetingsettings-resource-type"></a><span data-ttu-id="91e40-103">Тип ресурса broadcastMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="91e40-103">broadcastMeetingSettings resource type</span></span>

<span data-ttu-id="91e40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91e40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91e40-105">Параметры, связанные с трансляцией.</span><span class="sxs-lookup"><span data-stu-id="91e40-105">Settings related to a live event.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="91e40-106">Этот API не проверяет параметры трансляций, управляемые [политикой.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="91e40-106">This API does not validate live event settings that are managed by [policy](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).</span></span>
> <span data-ttu-id="91e40-107">Например, если администратор задает политику трансляций с помощью, пользователям будет запрещено устанавливать разрешения трансляций в клиенте Teams, но они смогут создавать трансляции с помощью Microsoft Graph, задав для `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** параметр `everyone` .</span><span class="sxs-lookup"><span data-stu-id="91e40-107">For example, if an admin sets a live event policy using `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany`, users will be prevented from setting live event permissions to `public` in their Teams client, but will be able to create a live event via Microsoft Graph by setting **allowedAudience** to `everyone`.</span></span> 

## <a name="properties"></a><span data-ttu-id="91e40-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91e40-108">Properties</span></span>

| <span data-ttu-id="91e40-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91e40-109">Property</span></span>                   | <span data-ttu-id="91e40-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91e40-110">Type</span></span>                     | <span data-ttu-id="91e40-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91e40-111">Description</span></span>                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| <span data-ttu-id="91e40-112">allowedAudience</span><span class="sxs-lookup"><span data-stu-id="91e40-112">allowedAudience</span></span>            | <span data-ttu-id="91e40-113">broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="91e40-113">broadcastMeetingAudience</span></span> | <span data-ttu-id="91e40-114">Определяет, кто может присоединиться к трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-114">Defines who can join the live event.</span></span> <span data-ttu-id="91e40-115">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="91e40-115">Possible values are listed in the following table.</span></span> |
| <span data-ttu-id="91e40-116">isRecordingEnabled</span><span class="sxs-lookup"><span data-stu-id="91e40-116">isRecordingEnabled</span></span>         | <span data-ttu-id="91e40-117">Логический</span><span class="sxs-lookup"><span data-stu-id="91e40-117">Boolean</span></span>                  | <span data-ttu-id="91e40-118">Указывает, включена ли запись для этого трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-118">Indicates whether recording is enabled for this live event.</span></span> <span data-ttu-id="91e40-119">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="91e40-119">Default value is `false`.</span></span>          |
| <span data-ttu-id="91e40-120">isAttendeeReportEnabled</span><span class="sxs-lookup"><span data-stu-id="91e40-120">isAttendeeReportEnabled</span></span>    | <span data-ttu-id="91e40-121">Логический</span><span class="sxs-lookup"><span data-stu-id="91e40-121">Boolean</span></span>                  | <span data-ttu-id="91e40-122">Указывает, включен ли отчет участника для этого трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-122">Indicates whether attendee report is enabled for this live event.</span></span> <span data-ttu-id="91e40-123">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="91e40-123">Default value is `false`.</span></span>    |
| <span data-ttu-id="91e40-124">isQuestionAndAnswerEnabled</span><span class="sxs-lookup"><span data-stu-id="91e40-124">isQuestionAndAnswerEnabled</span></span> | <span data-ttu-id="91e40-125">Логический</span><span class="sxs-lookup"><span data-stu-id="91e40-125">Boolean</span></span>                  | <span data-ttu-id="91e40-126">Указывает, включен ли вопрос&A для этого трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-126">Indicates whether Q&A is enabled for this live event.</span></span> <span data-ttu-id="91e40-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="91e40-127">Default value is `false`.</span></span>                |
| <span data-ttu-id="91e40-128">isVideoOnDemandEnabled</span><span class="sxs-lookup"><span data-stu-id="91e40-128">isVideoOnDemandEnabled</span></span>     | <span data-ttu-id="91e40-129">Логический</span><span class="sxs-lookup"><span data-stu-id="91e40-129">Boolean</span></span>                  | <span data-ttu-id="91e40-130">Указывает, включено ли видео по требованию для этого трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-130">Indicates whether video on demand is enabled for this live event.</span></span> <span data-ttu-id="91e40-131">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="91e40-131">Default value is `false`.</span></span>    |

### <a name="broadcastmeetingaudience-values"></a><span data-ttu-id="91e40-132">Значения broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="91e40-132">broadcastMeetingAudience values</span></span>

| <span data-ttu-id="91e40-133">Значение</span><span class="sxs-lookup"><span data-stu-id="91e40-133">Value</span></span>              | <span data-ttu-id="91e40-134">Описание</span><span class="sxs-lookup"><span data-stu-id="91e40-134">Description</span></span>                                                       |
| ------------------ | ----------------------------------------------------------------- |
| <span data-ttu-id="91e40-135">все</span><span class="sxs-lookup"><span data-stu-id="91e40-135">everyone</span></span>           | <span data-ttu-id="91e40-136">Трансляция будет открыта для всех.</span><span class="sxs-lookup"><span data-stu-id="91e40-136">The live event will be open to anyone.</span></span> <span data-ttu-id="91e40-137">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="91e40-137">This is the default value.</span></span> |
| <span data-ttu-id="91e40-138">organization;</span><span class="sxs-lookup"><span data-stu-id="91e40-138">organization</span></span>       | <span data-ttu-id="91e40-139">Все в вашей организации могут присоединиться к трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-139">Everyone in your org can join the live event.</span></span>                     |
| <span data-ttu-id="91e40-140">roleIsAttendee</span><span class="sxs-lookup"><span data-stu-id="91e40-140">roleIsAttendee</span></span>     | <span data-ttu-id="91e40-141">Только указанные люди могут присоединиться к трансляции.</span><span class="sxs-lookup"><span data-stu-id="91e40-141">Only the specified people can join the live event.</span></span>                |
| <span data-ttu-id="91e40-142">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="91e40-142">unknownFutureValue</span></span> | <span data-ttu-id="91e40-143">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="91e40-143">Unknown future value.</span></span>                                             |

## <a name="json-representation"></a><span data-ttu-id="91e40-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91e40-144">JSON representation</span></span>

<span data-ttu-id="91e40-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91e40-145">The following is a JSON representation of the resource.</span></span>

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
