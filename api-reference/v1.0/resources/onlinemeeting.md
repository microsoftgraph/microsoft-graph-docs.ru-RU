---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 812f094667b217d167509be324843227e552e0a5
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556228"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="a6da6-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-103">onlineMeeting resource type</span></span>

<span data-ttu-id="a6da6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6da6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6da6-105">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="a6da6-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="a6da6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a6da6-106">Methods</span></span>

| <span data-ttu-id="a6da6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a6da6-107">Method</span></span>         | <span data-ttu-id="a6da6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6da6-108">Return Type</span></span> | <span data-ttu-id="a6da6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6da6-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="a6da6-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a6da6-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="a6da6-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a6da6-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="a6da6-112">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="a6da6-113">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="a6da6-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a6da6-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="a6da6-115">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="a6da6-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="a6da6-116">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="a6da6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a6da6-117">None</span></span> | <span data-ttu-id="a6da6-118">Удаление собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-118">Delete an online meeting.</span></span> |
| [<span data-ttu-id="a6da6-119">Создание или получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="a6da6-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a6da6-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="a6da6-121">Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="a6da6-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="a6da6-122">Если собрание уже существует, извлеките его свойства.</span><span class="sxs-lookup"><span data-stu-id="a6da6-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6da6-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6da6-123">Properties</span></span>

| <span data-ttu-id="a6da6-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6da6-124">Property</span></span>                  | <span data-ttu-id="a6da6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a6da6-125">Type</span></span>                                                   | <span data-ttu-id="a6da6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a6da6-126">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a6da6-127">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-127">audioConferencing</span></span>         | [<span data-ttu-id="a6da6-128">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="a6da6-128">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="a6da6-129">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="a6da6-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-130">Read-only.</span></span> |
| <span data-ttu-id="a6da6-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="a6da6-131">chatInfo</span></span>                  | [<span data-ttu-id="a6da6-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="a6da6-132">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="a6da6-133">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-133">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="a6da6-134">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="a6da6-134">creationDateTime</span></span>          | <span data-ttu-id="a6da6-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="a6da6-135">DateTime</span></span>                                               | <span data-ttu-id="a6da6-136">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a6da6-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="a6da6-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-137">Read-only.</span></span> |
| <span data-ttu-id="a6da6-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a6da6-138">startDateTime</span></span>             | <span data-ttu-id="a6da6-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="a6da6-139">DateTime</span></span>                                               | <span data-ttu-id="a6da6-140">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a6da6-140">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="a6da6-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a6da6-141">endDateTime</span></span>               | <span data-ttu-id="a6da6-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="a6da6-142">DateTime</span></span>                                               | <span data-ttu-id="a6da6-143">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a6da6-143">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="a6da6-144">id</span><span class="sxs-lookup"><span data-stu-id="a6da6-144">id</span></span>                        | <span data-ttu-id="a6da6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="a6da6-145">String</span></span>                                                 | <span data-ttu-id="a6da6-146">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="a6da6-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-147">Read-only.</span></span> |
| <span data-ttu-id="a6da6-148">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="a6da6-148">joinWebUrl</span></span>                | <span data-ttu-id="a6da6-149">String</span><span class="sxs-lookup"><span data-stu-id="a6da6-149">String</span></span>                                                 | <span data-ttu-id="a6da6-150">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-150">The join URL of the online meeting.</span></span> <span data-ttu-id="a6da6-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-151">Read-only.</span></span>|
| <span data-ttu-id="a6da6-152">participants</span><span class="sxs-lookup"><span data-stu-id="a6da6-152">participants</span></span>              | [<span data-ttu-id="a6da6-153">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="a6da6-153">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="a6da6-154">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="a6da6-155">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="a6da6-155">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="a6da6-156">subject</span><span class="sxs-lookup"><span data-stu-id="a6da6-156">subject</span></span>                   | <span data-ttu-id="a6da6-157">String</span><span class="sxs-lookup"><span data-stu-id="a6da6-157">String</span></span>                                                 | <span data-ttu-id="a6da6-158">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="a6da6-158">The subject of the online meeting.</span></span> |
| <span data-ttu-id="a6da6-159">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="a6da6-159">videoTeleconferenceId</span></span>     | <span data-ttu-id="a6da6-160">String</span><span class="sxs-lookup"><span data-stu-id="a6da6-160">String</span></span>                                                 | <span data-ttu-id="a6da6-161">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="a6da6-161">The video teleconferencing ID.</span></span> <span data-ttu-id="a6da6-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-162">Read-only.</span></span> |
| <span data-ttu-id="a6da6-163">жоининформатион</span><span class="sxs-lookup"><span data-stu-id="a6da6-163">joinInformation</span></span> | [<span data-ttu-id="a6da6-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="a6da6-164">itemBody</span></span>](itembody.md) | <span data-ttu-id="a6da6-165">Сведения о присоединении на языке и языковом варианте, указанном в `Accept-Language` HTTP-заголовке Request.</span><span class="sxs-lookup"><span data-stu-id="a6da6-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="a6da6-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6da6-166">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6da6-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6da6-167">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String"
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
