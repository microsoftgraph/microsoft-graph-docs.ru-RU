---
title: Тип ресурса onlineMeeting
description: Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519600"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="b0acf-103">Тип ресурса onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b0acf-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0acf-104">Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="b0acf-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="b0acf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b0acf-105">Methods</span></span>

| <span data-ttu-id="b0acf-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b0acf-106">Method</span></span>         | <span data-ttu-id="b0acf-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0acf-107">Return Type</span></span> | <span data-ttu-id="b0acf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b0acf-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="b0acf-109">Получение onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b0acf-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="b0acf-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b0acf-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b0acf-111">Чтение свойства и связи объекта onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="b0acf-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0acf-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0acf-112">Properties</span></span>

| <span data-ttu-id="b0acf-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0acf-113">Property</span></span>                  | <span data-ttu-id="b0acf-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b0acf-114">Type</span></span>                                                   | <span data-ttu-id="b0acf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b0acf-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b0acf-116">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="b0acf-116">accessLevel</span></span>               | <span data-ttu-id="b0acf-117">String</span><span class="sxs-lookup"><span data-stu-id="b0acf-117">String</span></span>                                                 | <span data-ttu-id="b0acf-118">Уровень доступа, который управляет допуска на собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="b0acf-119">Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b0acf-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="b0acf-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b0acf-120">audioConferencing</span></span>         | [<span data-ttu-id="b0acf-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b0acf-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="b0acf-122">Представляет телефона данные для доступа к onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="b0acf-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="b0acf-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-123">canceledDateTime</span></span>          | <span data-ttu-id="b0acf-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-124">DateTime</span></span>                                               | <span data-ttu-id="b0acf-125">Время, когда приглашение на собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="b0acf-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="b0acf-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b0acf-126">chatInfo</span></span>                  | [<span data-ttu-id="b0acf-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b0acf-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="b0acf-128">Chat, связанного с этого собрания.</span><span class="sxs-lookup"><span data-stu-id="b0acf-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="b0acf-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-129">creationDateTime</span></span>          | <span data-ttu-id="b0acf-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-130">DateTime</span></span>                                               | <span data-ttu-id="b0acf-131">Время создания собрания.</span><span class="sxs-lookup"><span data-stu-id="b0acf-131">The time when the meeting was created.</span></span> <span data-ttu-id="b0acf-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0acf-132">Readonly.</span></span>
| <span data-ttu-id="b0acf-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-133">endDateTime</span></span>               | <span data-ttu-id="b0acf-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-134">DateTime</span></span>                                               | <span data-ttu-id="b0acf-135">Время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="b0acf-135">End time of the meeting.</span></span> |
| <span data-ttu-id="b0acf-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="b0acf-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="b0acf-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="b0acf-137">Boolean</span></span>                                                | <span data-ttu-id="b0acf-138">Состояние присутствия объявлений для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="b0acf-139">При включении извещения присутствия собрание по сети объявлять имена participantswho join в собрании по аудио.</span><span class="sxs-lookup"><span data-stu-id="b0acf-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="b0acf-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-140">expirationDateTime</span></span>        | <span data-ttu-id="b0acf-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-141">DateTime</span></span>                                               | <span data-ttu-id="b0acf-142">Абсолютный по Гринвичу (UTC) даты и времени, после которого можно удалить собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="b0acf-143">Даты и времени должны быть от одного года до до десять лет после текущей датой и временем на сервере.</span><span class="sxs-lookup"><span data-stu-id="b0acf-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="b0acf-144">id</span><span class="sxs-lookup"><span data-stu-id="b0acf-144">id</span></span>                        | <span data-ttu-id="b0acf-145">String</span><span class="sxs-lookup"><span data-stu-id="b0acf-145">String</span></span>                                                 | <span data-ttu-id="b0acf-146">Идентификатор, связанный с собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="b0acf-147">Используется в начало HTTP-запросов в качестве идентификатора.</span><span class="sxs-lookup"><span data-stu-id="b0acf-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="b0acf-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0acf-148">Read-only.</span></span> <span data-ttu-id="b0acf-149">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="b0acf-149">Server generated.</span></span> |
| <span data-ttu-id="b0acf-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="b0acf-150">isCancelled</span></span>               | <span data-ttu-id="b0acf-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0acf-151">Boolean</span></span>                                                | <span data-ttu-id="b0acf-152">Приглашение на собрание была ли отменена.</span><span class="sxs-lookup"><span data-stu-id="b0acf-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="b0acf-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="b0acf-153">joinUrl</span></span>                   | <span data-ttu-id="b0acf-154">String</span><span class="sxs-lookup"><span data-stu-id="b0acf-154">String</span></span>                                                 | <span data-ttu-id="b0acf-155">URL-адрес, используемый при собрание по сети, связанное с веб.</span><span class="sxs-lookup"><span data-stu-id="b0acf-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="b0acf-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="b0acf-156">meetingType</span></span>               | <span data-ttu-id="b0acf-157">String</span><span class="sxs-lookup"><span data-stu-id="b0acf-157">String</span></span>                                                 | <span data-ttu-id="b0acf-158">Возможные значения: `meetNow`, `scheduled`, `recurring`.</span><span class="sxs-lookup"><span data-stu-id="b0acf-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="b0acf-159">participants</span><span class="sxs-lookup"><span data-stu-id="b0acf-159">participants</span></span>              | [<span data-ttu-id="b0acf-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="b0acf-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="b0acf-161">Участники, связанные с собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="b0acf-162">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="b0acf-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="b0acf-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-163">startDateTime</span></span>             | <span data-ttu-id="b0acf-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="b0acf-164">DateTime</span></span>                                               | <span data-ttu-id="b0acf-165">Запустите время собрания.</span><span class="sxs-lookup"><span data-stu-id="b0acf-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="b0acf-166">subject</span><span class="sxs-lookup"><span data-stu-id="b0acf-166">subject</span></span>                   | <span data-ttu-id="b0acf-167">String</span><span class="sxs-lookup"><span data-stu-id="b0acf-167">String</span></span>                                                 | <span data-ttu-id="b0acf-168">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="b0acf-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b0acf-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0acf-169">Relationships</span></span>
<span data-ttu-id="b0acf-170">Нет</span><span class="sxs-lookup"><span data-stu-id="b0acf-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0acf-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0acf-171">JSON representation</span></span>

<span data-ttu-id="b0acf-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0acf-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
