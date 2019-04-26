---
title: Тип ресурса Онлинемитинг
description: Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 698058fa918462448fcd115d5573e13ada49162e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341843"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="2d8d9-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="2d8d9-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d8d9-104">Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="2d8d9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2d8d9-105">Methods</span></span>

| <span data-ttu-id="2d8d9-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2d8d9-106">Method</span></span>         | <span data-ttu-id="2d8d9-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d8d9-107">Return Type</span></span> | <span data-ttu-id="2d8d9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8d9-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="2d8d9-109">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="2d8d9-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="2d8d9-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="2d8d9-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="2d8d9-111">Чтение свойств и связей объекта Онлинемитинг.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d8d9-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d8d9-112">Properties</span></span>

| <span data-ttu-id="2d8d9-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d8d9-113">Property</span></span>                  | <span data-ttu-id="2d8d9-114">Тип</span><span class="sxs-lookup"><span data-stu-id="2d8d9-114">Type</span></span>                                                   | <span data-ttu-id="2d8d9-115">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8d9-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2d8d9-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2d8d9-116">accessLevel</span></span>               | <span data-ttu-id="2d8d9-117">String</span><span class="sxs-lookup"><span data-stu-id="2d8d9-117">String</span></span>                                                 | <span data-ttu-id="2d8d9-118">Уровень доступа, который управляет допуском собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="2d8d9-119">Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="2d8d9-120">АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="2d8d9-120">audioConferencing</span></span>         | [<span data-ttu-id="2d8d9-121">АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="2d8d9-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="2d8d9-122">Представляет сведения о доступе к телефонии для Онлинемитинг.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="2d8d9-123">Канцеледдатетиме</span><span class="sxs-lookup"><span data-stu-id="2d8d9-123">canceledDateTime</span></span>          | <span data-ttu-id="2d8d9-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-124">DateTime</span></span>                                               | <span data-ttu-id="2d8d9-125">Время, когда собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="2d8d9-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="2d8d9-126">chatInfo</span></span>                  | [<span data-ttu-id="2d8d9-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="2d8d9-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="2d8d9-128">Чат, связанный с этим собранием.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="2d8d9-129">Креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="2d8d9-129">creationDateTime</span></span>          | <span data-ttu-id="2d8d9-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-130">DateTime</span></span>                                               | <span data-ttu-id="2d8d9-131">Время создания собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-131">The time when the meeting was created.</span></span> <span data-ttu-id="2d8d9-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-132">Read-only.</span></span>
| <span data-ttu-id="2d8d9-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-133">endDateTime</span></span>               | <span data-ttu-id="2d8d9-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-134">DateTime</span></span>                                               | <span data-ttu-id="2d8d9-135">Время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-135">End time of the meeting.</span></span> |
| <span data-ttu-id="2d8d9-136">Ентрекситаннаунцемент</span><span class="sxs-lookup"><span data-stu-id="2d8d9-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="2d8d9-137">Логический</span><span class="sxs-lookup"><span data-stu-id="2d8d9-137">Boolean</span></span>                                                | <span data-ttu-id="2d8d9-138">Состояние объявления о присутствии для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="2d8d9-139">Если объявления о присутствии включены, собрание по сети будет объявлять об именах участников, которые присоединяются к собранию с помощью звука.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-139">When attendance announcements are enabled, the online meeting will announce the names of the participants who join the meeting through audio.</span></span> |
| <span data-ttu-id="2d8d9-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-140">expirationDateTime</span></span>        | <span data-ttu-id="2d8d9-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-141">DateTime</span></span>                                               | <span data-ttu-id="2d8d9-142">Дата и время, по истечении которого собрание по сети может быть удалено в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="2d8d9-143">День и время должны находиться в пределах одного года до и десяти лет после текущей даты и времени на сервере.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="2d8d9-144">id</span><span class="sxs-lookup"><span data-stu-id="2d8d9-144">id</span></span>                        | <span data-ttu-id="2d8d9-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2d8d9-145">String</span></span>                                                 | <span data-ttu-id="2d8d9-146">Идентификатор, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="2d8d9-147">Используется в запросе GET HTTP в качестве идентификатора.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="2d8d9-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-148">Read-only.</span></span> <span data-ttu-id="2d8d9-149">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-149">Server generated.</span></span> |
| <span data-ttu-id="2d8d9-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="2d8d9-150">isCancelled</span></span>               | <span data-ttu-id="2d8d9-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d8d9-151">Boolean</span></span>                                                | <span data-ttu-id="2d8d9-152">Указывает, было ли собрание отменено.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="2d8d9-153">Жоинурл</span><span class="sxs-lookup"><span data-stu-id="2d8d9-153">joinUrl</span></span>                   | <span data-ttu-id="2d8d9-154">String</span><span class="sxs-lookup"><span data-stu-id="2d8d9-154">String</span></span>                                                 | <span data-ttu-id="2d8d9-155">URL-адрес, используемый при присоединении собрания по сети из Интернета.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="2d8d9-156">Митингтипе</span><span class="sxs-lookup"><span data-stu-id="2d8d9-156">meetingType</span></span>               | <span data-ttu-id="2d8d9-157">String</span><span class="sxs-lookup"><span data-stu-id="2d8d9-157">String</span></span>                                                 | <span data-ttu-id="2d8d9-158">Возможные `meetNow`значения:, `scheduled`, `recurring`, `broadcast` (Примечание: [CREATE онлинемитинг](../api/application-post-onlinemeetings.md) поддерживает `meetNow`только).</span><span class="sxs-lookup"><span data-stu-id="2d8d9-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast` (Note: [create onlineMeeting](../api/application-post-onlinemeetings.md) only supports `meetNow`).</span></span> |
| <span data-ttu-id="2d8d9-159">participants</span><span class="sxs-lookup"><span data-stu-id="2d8d9-159">participants</span></span>              | [<span data-ttu-id="2d8d9-160">МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="2d8d9-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="2d8d9-161">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="2d8d9-162">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="2d8d9-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-163">startDateTime</span></span>             | <span data-ttu-id="2d8d9-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d8d9-164">DateTime</span></span>                                               | <span data-ttu-id="2d8d9-165">Время начала собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="2d8d9-166">subject</span><span class="sxs-lookup"><span data-stu-id="2d8d9-166">subject</span></span>                   | <span data-ttu-id="2d8d9-167">String</span><span class="sxs-lookup"><span data-stu-id="2d8d9-167">String</span></span>                                                 | <span data-ttu-id="2d8d9-168">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d8d9-169">Связи</span><span class="sxs-lookup"><span data-stu-id="2d8d9-169">Relationships</span></span>
<span data-ttu-id="2d8d9-170">Нет</span><span class="sxs-lookup"><span data-stu-id="2d8d9-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d8d9-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d8d9-171">JSON representation</span></span>

<span data-ttu-id="2d8d9-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d8d9-172">The following is a JSON representation of the resource.</span></span>

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