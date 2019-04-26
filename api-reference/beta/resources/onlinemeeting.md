---
title: Тип ресурса Онлинемитинг
description: Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568867"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="8bdea-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="8bdea-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bdea-104">Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.</span><span class="sxs-lookup"><span data-stu-id="8bdea-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="8bdea-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8bdea-105">Methods</span></span>

| <span data-ttu-id="8bdea-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8bdea-106">Method</span></span>         | <span data-ttu-id="8bdea-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bdea-107">Return Type</span></span> | <span data-ttu-id="8bdea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8bdea-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="8bdea-109">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="8bdea-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="8bdea-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8bdea-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="8bdea-111">Чтение свойств и связей объекта Онлинемитинг.</span><span class="sxs-lookup"><span data-stu-id="8bdea-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8bdea-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bdea-112">Properties</span></span>

| <span data-ttu-id="8bdea-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bdea-113">Property</span></span>                  | <span data-ttu-id="8bdea-114">Тип</span><span class="sxs-lookup"><span data-stu-id="8bdea-114">Type</span></span>                                                   | <span data-ttu-id="8bdea-115">Описание</span><span class="sxs-lookup"><span data-stu-id="8bdea-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8bdea-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="8bdea-116">accessLevel</span></span>               | <span data-ttu-id="8bdea-117">String</span><span class="sxs-lookup"><span data-stu-id="8bdea-117">String</span></span>                                                 | <span data-ttu-id="8bdea-118">Уровень доступа, который управляет допуском собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="8bdea-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="8bdea-119">Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8bdea-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="8bdea-120">АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="8bdea-120">audioConferencing</span></span>         | [<span data-ttu-id="8bdea-121">АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="8bdea-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="8bdea-122">Представляет сведения о доступе к телефонии для Онлинемитинг.</span><span class="sxs-lookup"><span data-stu-id="8bdea-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="8bdea-123">Канцеледдатетиме</span><span class="sxs-lookup"><span data-stu-id="8bdea-123">canceledDateTime</span></span>          | <span data-ttu-id="8bdea-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-124">DateTime</span></span>                                               | <span data-ttu-id="8bdea-125">Время, когда собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="8bdea-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="8bdea-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8bdea-126">chatInfo</span></span>                  | [<span data-ttu-id="8bdea-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8bdea-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="8bdea-128">Чат, связанный с этим собранием.</span><span class="sxs-lookup"><span data-stu-id="8bdea-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="8bdea-129">Креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="8bdea-129">creationDateTime</span></span>          | <span data-ttu-id="8bdea-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-130">DateTime</span></span>                                               | <span data-ttu-id="8bdea-131">Время создания собрания.</span><span class="sxs-lookup"><span data-stu-id="8bdea-131">The time when the meeting was created.</span></span> <span data-ttu-id="8bdea-132">Статического.</span><span class="sxs-lookup"><span data-stu-id="8bdea-132">Readonly.</span></span>
| <span data-ttu-id="8bdea-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-133">endDateTime</span></span>               | <span data-ttu-id="8bdea-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-134">DateTime</span></span>                                               | <span data-ttu-id="8bdea-135">Время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="8bdea-135">End time of the meeting.</span></span> |
| <span data-ttu-id="8bdea-136">Ентрекситаннаунцемент</span><span class="sxs-lookup"><span data-stu-id="8bdea-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="8bdea-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bdea-137">Boolean</span></span>                                                | <span data-ttu-id="8bdea-138">Состояние объявления о присутствии для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="8bdea-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="8bdea-139">Если объявления о присутствии включены, собрание по сети будет объявлять об именах партиЦипантсвхо, присоединяющихся к собранию с помощью звука.</span><span class="sxs-lookup"><span data-stu-id="8bdea-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="8bdea-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-140">expirationDateTime</span></span>        | <span data-ttu-id="8bdea-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-141">DateTime</span></span>                                               | <span data-ttu-id="8bdea-142">Дата и время, по истечении которого собрание по сети может быть удалено в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8bdea-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="8bdea-143">День и время должны находиться в пределах одного года до и десяти лет после текущей даты и времени на сервере.</span><span class="sxs-lookup"><span data-stu-id="8bdea-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="8bdea-144">id</span><span class="sxs-lookup"><span data-stu-id="8bdea-144">id</span></span>                        | <span data-ttu-id="8bdea-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdea-145">String</span></span>                                                 | <span data-ttu-id="8bdea-146">Идентификатор, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="8bdea-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="8bdea-147">Используется в запросе GET HTTP в качестве идентификатора.</span><span class="sxs-lookup"><span data-stu-id="8bdea-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="8bdea-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bdea-148">Read-only.</span></span> <span data-ttu-id="8bdea-149">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="8bdea-149">Server generated.</span></span> |
| <span data-ttu-id="8bdea-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="8bdea-150">isCancelled</span></span>               | <span data-ttu-id="8bdea-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bdea-151">Boolean</span></span>                                                | <span data-ttu-id="8bdea-152">Указывает, было ли собрание отменено.</span><span class="sxs-lookup"><span data-stu-id="8bdea-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="8bdea-153">Жоинурл</span><span class="sxs-lookup"><span data-stu-id="8bdea-153">joinUrl</span></span>                   | <span data-ttu-id="8bdea-154">String</span><span class="sxs-lookup"><span data-stu-id="8bdea-154">String</span></span>                                                 | <span data-ttu-id="8bdea-155">URL-адрес, используемый при присоединении собрания по сети из Интернета.</span><span class="sxs-lookup"><span data-stu-id="8bdea-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="8bdea-156">Митингтипе</span><span class="sxs-lookup"><span data-stu-id="8bdea-156">meetingType</span></span>               | <span data-ttu-id="8bdea-157">String</span><span class="sxs-lookup"><span data-stu-id="8bdea-157">String</span></span>                                                 | <span data-ttu-id="8bdea-158">Возможные значения: `meetNow`, `scheduled`,, `recurring``broadcast`</span><span class="sxs-lookup"><span data-stu-id="8bdea-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="8bdea-159">participants</span><span class="sxs-lookup"><span data-stu-id="8bdea-159">participants</span></span>              | [<span data-ttu-id="8bdea-160">МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="8bdea-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="8bdea-161">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="8bdea-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="8bdea-162">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="8bdea-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="8bdea-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-163">startDateTime</span></span>             | <span data-ttu-id="8bdea-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="8bdea-164">DateTime</span></span>                                               | <span data-ttu-id="8bdea-165">Время начала собрания.</span><span class="sxs-lookup"><span data-stu-id="8bdea-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="8bdea-166">subject</span><span class="sxs-lookup"><span data-stu-id="8bdea-166">subject</span></span>                   | <span data-ttu-id="8bdea-167">String</span><span class="sxs-lookup"><span data-stu-id="8bdea-167">String</span></span>                                                 | <span data-ttu-id="8bdea-168">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="8bdea-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8bdea-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="8bdea-169">Relationships</span></span>
<span data-ttu-id="8bdea-170">Нет</span><span class="sxs-lookup"><span data-stu-id="8bdea-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bdea-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bdea-171">JSON representation</span></span>

<span data-ttu-id="8bdea-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bdea-172">The following is a JSON representation of the resource.</span></span>

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
