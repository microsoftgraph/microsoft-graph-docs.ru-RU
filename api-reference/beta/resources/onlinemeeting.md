---
title: Тип ресурса onlineMeeting
description: Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.
ms.openlocfilehash: 73e45f7f2c04df469f2c2fb0faf1c8a0f8680a64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075753"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="6f495-103">Тип ресурса onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6f495-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="6f495-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f495-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f495-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f495-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f495-106">Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="6f495-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="6f495-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6f495-107">Methods</span></span>

| <span data-ttu-id="6f495-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6f495-108">Method</span></span>         | <span data-ttu-id="6f495-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f495-109">Return Type</span></span> | <span data-ttu-id="6f495-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f495-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="6f495-111">Получение onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6f495-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="6f495-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6f495-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6f495-113">Чтение свойства и связи объекта onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="6f495-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f495-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f495-114">Properties</span></span>

| <span data-ttu-id="6f495-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f495-115">Property</span></span>                  | <span data-ttu-id="6f495-116">Тип</span><span class="sxs-lookup"><span data-stu-id="6f495-116">Type</span></span>                                                   | <span data-ttu-id="6f495-117">Description</span><span class="sxs-lookup"><span data-stu-id="6f495-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6f495-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="6f495-118">accessLevel</span></span>               | <span data-ttu-id="6f495-119">String</span><span class="sxs-lookup"><span data-stu-id="6f495-119">String</span></span>                                                 | <span data-ttu-id="6f495-120">Уровень доступа, который управляет допуска на собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="6f495-121">Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6f495-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="6f495-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="6f495-122">audioConferencing</span></span>         | [<span data-ttu-id="6f495-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="6f495-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="6f495-124">Представляет телефона данные для доступа к onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="6f495-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="6f495-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-125">canceledDateTime</span></span>          | <span data-ttu-id="6f495-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-126">DateTime</span></span>                                               | <span data-ttu-id="6f495-127">Время, когда приглашение на собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="6f495-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="6f495-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6f495-128">chatInfo</span></span>                  | [<span data-ttu-id="6f495-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6f495-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="6f495-130">Chat, связанного с этого собрания.</span><span class="sxs-lookup"><span data-stu-id="6f495-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="6f495-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-131">creationDateTime</span></span>          | <span data-ttu-id="6f495-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-132">DateTime</span></span>                                               | <span data-ttu-id="6f495-133">Время создания собрания.</span><span class="sxs-lookup"><span data-stu-id="6f495-133">The time when the meeting was created.</span></span> <span data-ttu-id="6f495-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f495-134">Readonly.</span></span>
| <span data-ttu-id="6f495-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-135">endDateTime</span></span>               | <span data-ttu-id="6f495-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-136">DateTime</span></span>                                               | <span data-ttu-id="6f495-137">Время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="6f495-137">End time of the meeting.</span></span> |
| <span data-ttu-id="6f495-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="6f495-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="6f495-139">Логический</span><span class="sxs-lookup"><span data-stu-id="6f495-139">Boolean</span></span>                                                | <span data-ttu-id="6f495-140">Состояние присутствия объявлений для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="6f495-141">При включении извещения присутствия собрание по сети объявлять имена participantswho join в собрании по аудио.</span><span class="sxs-lookup"><span data-stu-id="6f495-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="6f495-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-142">expirationDateTime</span></span>        | <span data-ttu-id="6f495-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-143">DateTime</span></span>                                               | <span data-ttu-id="6f495-144">Абсолютный по Гринвичу (UTC) даты и времени, после которого можно удалить собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="6f495-145">Даты и времени должны быть от одного года до до десять лет после текущей датой и временем на сервере.</span><span class="sxs-lookup"><span data-stu-id="6f495-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="6f495-146">id</span><span class="sxs-lookup"><span data-stu-id="6f495-146">id</span></span>                        | <span data-ttu-id="6f495-147">String</span><span class="sxs-lookup"><span data-stu-id="6f495-147">String</span></span>                                                 | <span data-ttu-id="6f495-148">Идентификатор, связанный с собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="6f495-149">Используется в начало HTTP-запросов в качестве идентификатора.</span><span class="sxs-lookup"><span data-stu-id="6f495-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="6f495-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f495-150">Read-only.</span></span> <span data-ttu-id="6f495-151">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="6f495-151">Server generated.</span></span> |
| <span data-ttu-id="6f495-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="6f495-152">isCancelled</span></span>               | <span data-ttu-id="6f495-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f495-153">Boolean</span></span>                                                | <span data-ttu-id="6f495-154">Приглашение на собрание была ли отменена.</span><span class="sxs-lookup"><span data-stu-id="6f495-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="6f495-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="6f495-155">joinUrl</span></span>                   | <span data-ttu-id="6f495-156">String</span><span class="sxs-lookup"><span data-stu-id="6f495-156">String</span></span>                                                 | <span data-ttu-id="6f495-157">URL-адрес, используемый при собрание по сети, связанное с веб.</span><span class="sxs-lookup"><span data-stu-id="6f495-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="6f495-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="6f495-158">meetingType</span></span>               | <span data-ttu-id="6f495-159">String</span><span class="sxs-lookup"><span data-stu-id="6f495-159">String</span></span>                                                 | <span data-ttu-id="6f495-160">Возможные значения: `meetNow`, `scheduled`, `recurring`,`broadcast`</span><span class="sxs-lookup"><span data-stu-id="6f495-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="6f495-161">participants</span><span class="sxs-lookup"><span data-stu-id="6f495-161">participants</span></span>              | [<span data-ttu-id="6f495-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="6f495-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="6f495-163">Участники, связанные с собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="6f495-164">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="6f495-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="6f495-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-165">startDateTime</span></span>             | <span data-ttu-id="6f495-166">DateTime</span><span class="sxs-lookup"><span data-stu-id="6f495-166">DateTime</span></span>                                               | <span data-ttu-id="6f495-167">Запустите время собрания.</span><span class="sxs-lookup"><span data-stu-id="6f495-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="6f495-168">subject</span><span class="sxs-lookup"><span data-stu-id="6f495-168">subject</span></span>                   | <span data-ttu-id="6f495-169">String</span><span class="sxs-lookup"><span data-stu-id="6f495-169">String</span></span>                                                 | <span data-ttu-id="6f495-170">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6f495-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6f495-171">Связи</span><span class="sxs-lookup"><span data-stu-id="6f495-171">Relationships</span></span>
<span data-ttu-id="6f495-172">Нет</span><span class="sxs-lookup"><span data-stu-id="6f495-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f495-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f495-173">JSON representation</span></span>

<span data-ttu-id="6f495-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f495-174">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
