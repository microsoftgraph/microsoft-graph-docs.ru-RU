---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 9f986bf0bd7871185673759a6e98e80d5d10b4b7
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741931"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="17460-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="17460-103">onlineMeeting resource type</span></span>

<span data-ttu-id="17460-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17460-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17460-105">Содержит сведения о собрании, в том числе URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="17460-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="17460-106">Методы</span><span class="sxs-lookup"><span data-stu-id="17460-106">Methods</span></span>

| <span data-ttu-id="17460-107">Метод</span><span class="sxs-lookup"><span data-stu-id="17460-107">Method</span></span>                                                             | <span data-ttu-id="17460-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17460-108">Return Type</span></span>                       | <span data-ttu-id="17460-109">Описание</span><span class="sxs-lookup"><span data-stu-id="17460-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="17460-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="17460-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="17460-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="17460-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="17460-112">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="17460-113">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="17460-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="17460-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="17460-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="17460-115">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="17460-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="17460-116">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="17460-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="17460-117">Нет</span><span class="sxs-lookup"><span data-stu-id="17460-117">None</span></span>                              | <span data-ttu-id="17460-118">Удаление собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="17460-119">Создание или получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="17460-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="17460-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="17460-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="17460-121">Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="17460-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="17460-122">Если собрание уже существует, извлеките его свойства.</span><span class="sxs-lookup"><span data-stu-id="17460-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="17460-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="17460-123">Properties</span></span>

| <span data-ttu-id="17460-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="17460-124">Property</span></span>              | <span data-ttu-id="17460-125">Тип</span><span class="sxs-lookup"><span data-stu-id="17460-125">Type</span></span>                                          | <span data-ttu-id="17460-126">Описание</span><span class="sxs-lookup"><span data-stu-id="17460-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="17460-127">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="17460-127">audioConferencing</span></span>     | [<span data-ttu-id="17460-128">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="17460-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="17460-129">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="17460-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="17460-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="17460-131">chatInfo</span></span>              | [<span data-ttu-id="17460-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="17460-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="17460-133">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="17460-134">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="17460-134">creationDateTime</span></span>      | <span data-ttu-id="17460-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="17460-135">DateTime</span></span>                                      | <span data-ttu-id="17460-136">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="17460-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="17460-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="17460-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="17460-138">startDateTime</span></span>         | <span data-ttu-id="17460-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="17460-139">DateTime</span></span>                                      | <span data-ttu-id="17460-140">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="17460-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="17460-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="17460-141">endDateTime</span></span>           | <span data-ttu-id="17460-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="17460-142">DateTime</span></span>                                      | <span data-ttu-id="17460-143">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="17460-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="17460-144">id</span><span class="sxs-lookup"><span data-stu-id="17460-144">id</span></span>                    | <span data-ttu-id="17460-145">String</span><span class="sxs-lookup"><span data-stu-id="17460-145">String</span></span>                                        | <span data-ttu-id="17460-146">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="17460-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="17460-148">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="17460-148">joinWebUrl</span></span>            | <span data-ttu-id="17460-149">String</span><span class="sxs-lookup"><span data-stu-id="17460-149">String</span></span>                                        | <span data-ttu-id="17460-150">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-150">The join URL of the online meeting.</span></span> <span data-ttu-id="17460-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="17460-152">participants</span><span class="sxs-lookup"><span data-stu-id="17460-152">participants</span></span>          | [<span data-ttu-id="17460-153">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="17460-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="17460-154">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="17460-155">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="17460-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="17460-156">subject</span><span class="sxs-lookup"><span data-stu-id="17460-156">subject</span></span>               | <span data-ttu-id="17460-157">String</span><span class="sxs-lookup"><span data-stu-id="17460-157">String</span></span>                                        | <span data-ttu-id="17460-158">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="17460-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="17460-159">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="17460-159">videoTeleconferenceId</span></span> | <span data-ttu-id="17460-160">String</span><span class="sxs-lookup"><span data-stu-id="17460-160">String</span></span>                                        | <span data-ttu-id="17460-161">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="17460-161">The video teleconferencing ID.</span></span> <span data-ttu-id="17460-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="17460-163">жоининформатион</span><span class="sxs-lookup"><span data-stu-id="17460-163">joinInformation</span></span>       | [<span data-ttu-id="17460-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="17460-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="17460-165">Сведения о присоединении на языке и языковом варианте, указанном в `Accept-Language` HTTP-заголовке Request.</span><span class="sxs-lookup"><span data-stu-id="17460-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="17460-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17460-166">Read-only.</span></span> |
| <span data-ttu-id="17460-167">исентрекситаннаунцед</span><span class="sxs-lookup"><span data-stu-id="17460-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="17460-168">Логический</span><span class="sxs-lookup"><span data-stu-id="17460-168">Boolean</span></span>                                       | <span data-ttu-id="17460-169">Указывает, следует ли объявлять, когда звонящие присоединяются или оставляют.</span><span class="sxs-lookup"><span data-stu-id="17460-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="17460-170">лоббибипасссеттингс</span><span class="sxs-lookup"><span data-stu-id="17460-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="17460-171">лоббибипасссеттингс</span><span class="sxs-lookup"><span data-stu-id="17460-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="17460-172">Указывает, какие участники могут обходить зал собрания.</span><span class="sxs-lookup"><span data-stu-id="17460-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                                 |
| <span data-ttu-id="17460-173">алловедпресентерс</span><span class="sxs-lookup"><span data-stu-id="17460-173">allowedPresenters</span></span>     | <span data-ttu-id="17460-174">онлинемитингпресентерс</span><span class="sxs-lookup"><span data-stu-id="17460-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="17460-175">Указывает, кто может быть докладчиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="17460-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="17460-176">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="17460-176">Possible values are listed in the following table.</span></span>                                           |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="17460-177">значения Онлинемитингпресентерс</span><span class="sxs-lookup"><span data-stu-id="17460-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="17460-178">Значение</span><span class="sxs-lookup"><span data-stu-id="17460-178">Value</span></span>              | <span data-ttu-id="17460-179">Описание</span><span class="sxs-lookup"><span data-stu-id="17460-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="17460-180">просматривающи</span><span class="sxs-lookup"><span data-stu-id="17460-180">everyone</span></span>           | <span data-ttu-id="17460-181">"Все" — докладчик (это параметр по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="17460-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="17460-182">organization;</span><span class="sxs-lookup"><span data-stu-id="17460-182">organization</span></span>       | <span data-ttu-id="17460-183">Все пользователи в Организации организатора — докладчик.</span><span class="sxs-lookup"><span data-stu-id="17460-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="17460-184">ролеиспресентер</span><span class="sxs-lookup"><span data-stu-id="17460-184">roleIsPresenter</span></span>    | <span data-ttu-id="17460-185">Докладчиками являются только те участники, у которых есть роль докладчика.</span><span class="sxs-lookup"><span data-stu-id="17460-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="17460-186">organizer</span><span class="sxs-lookup"><span data-stu-id="17460-186">organizer</span></span>          | <span data-ttu-id="17460-187">Только организатор является выступающим.</span><span class="sxs-lookup"><span data-stu-id="17460-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="17460-188">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="17460-188">unknownFutureValue</span></span> | <span data-ttu-id="17460-189">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="17460-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="17460-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17460-190">JSON representation</span></span>

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
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

