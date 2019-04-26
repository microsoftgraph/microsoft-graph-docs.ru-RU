---
title: Тип ресурса "упоминание"
description: Представляет уведомление для пользователя на основе электронного адреса пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 28a77b393f2d5574453d08b93df487ffc5203e2c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342326"
---
# <a name="mention-resource-type"></a><span data-ttu-id="8f876-103">Тип ресурса "упоминание"</span><span class="sxs-lookup"><span data-stu-id="8f876-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f876-104">Представляет уведомление для пользователя на основе электронного адреса пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="8f876-105">Этот тип уведомления также называется @-упоминаниями.</span><span class="sxs-lookup"><span data-stu-id="8f876-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="8f876-106">Ресурс [Message](../resources/message.md) поддерживает **упоминание**.</span><span class="sxs-lookup"><span data-stu-id="8f876-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="8f876-107">Он включает свойство **ментионспревиев** , которое указывает, упоминается ли вошедшего в данный экземпляр сообщения пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="8f876-108">Кроме того, он \*\*\*\* включает свойство навигации упоминаютй, которое поддерживает сбор сведений о упоминании или удаление упоминания в этом экземпляре.</span><span class="sxs-lookup"><span data-stu-id="8f876-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="8f876-109">При создании сообщения приложение может создать упоминание в том же `POST` запросе, включив в свойство **упоминаются** упоминание.</span><span class="sxs-lookup"><span data-stu-id="8f876-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="8f876-110">С помощью `GET` запроса с параметром `$filter` Query приложение может возвратить все сообщения в почтовом ящике вошедшего пользователя, который упоминает пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="8f876-111">`GET` Запрос с параметром `$expand` запроса позволяет приложению развернуть все упоминания в определенном сообщении.</span><span class="sxs-lookup"><span data-stu-id="8f876-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="8f876-112">Этот механизм, позволяющий приложениям устанавливать и получать упоминание в сообщениях, включает облегченные уведомления, где пользователь, проверяя упоминание, может находиться в существующем контексте (например, составление текста сообщения), пока приложение устанавливает базовое свойство **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="8f876-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="8f876-113">Упомянутые лица могут легко выяснить, где они упоминаются с помощью `GET` запросов с `$filter` параметром `$expand` или с помощью параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="8f876-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="8f876-114">Например, в почтовом клиенте Outlook, когда пользователь вводит `@` сообщение, Outlook позволяет пользователю выбрать или ввести имя для завершения @ – упоминаний.</span><span class="sxs-lookup"><span data-stu-id="8f876-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="8f876-115">Outlook задает \*\*\*\* свойство упоминаются перед созданием и отправкой сообщения или события.</span><span class="sxs-lookup"><span data-stu-id="8f876-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="8f876-116">Outlook также использует `GET` операции с `$filter` и `$expand` , чтобы пользователь, вошедшего в систему, мог выполнять поиск сообщений, которые упоминают пользователя, предупреждает пользователя о действиях или обсуждениях, что позволяет быстрее отреагировать на действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f876-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f876-117">JSON representation</span></span>

<span data-ttu-id="8f876-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f876-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a><span data-ttu-id="8f876-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f876-119">Properties</span></span>
| <span data-ttu-id="8f876-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f876-120">Property</span></span>     | <span data-ttu-id="8f876-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8f876-121">Type</span></span>   |<span data-ttu-id="8f876-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f876-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f876-123">application</span><span class="sxs-lookup"><span data-stu-id="8f876-123">application</span></span> | <span data-ttu-id="8f876-124">String</span><span class="sxs-lookup"><span data-stu-id="8f876-124">String</span></span> | <span data-ttu-id="8f876-125">Имя приложения, в котором создается упоминание.</span><span class="sxs-lookup"><span data-stu-id="8f876-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="8f876-126">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8f876-126">Optional.</span></span> <span data-ttu-id="8f876-127">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="8f876-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8f876-128">Клиентреференце</span><span class="sxs-lookup"><span data-stu-id="8f876-128">clientReference</span></span> | <span data-ttu-id="8f876-129">String</span><span class="sxs-lookup"><span data-stu-id="8f876-129">String</span></span> | <span data-ttu-id="8f876-130">Уникальный идентификатор, представляющий родительский объект для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="8f876-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="8f876-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8f876-131">Optional.</span></span> <span data-ttu-id="8f876-132">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="8f876-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8f876-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="8f876-133">createdBy</span></span>  | [<span data-ttu-id="8f876-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f876-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="8f876-135">Сведения электронной почты пользователя, выполнившего упоминание.</span><span class="sxs-lookup"><span data-stu-id="8f876-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="8f876-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f876-136">createdDateTime</span></span>  |<span data-ttu-id="8f876-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f876-137">DateTimeOffset</span></span> |<span data-ttu-id="8f876-138">Дата и время создания упоминания в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8f876-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="8f876-139">Прямой</span><span class="sxs-lookup"><span data-stu-id="8f876-139">deepLink</span></span> | <span data-ttu-id="8f876-140">String</span><span class="sxs-lookup"><span data-stu-id="8f876-140">String</span></span> | <span data-ttu-id="8f876-141">Глубокая веб-ссылка на контекст упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="8f876-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="8f876-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8f876-142">Optional.</span></span> <span data-ttu-id="8f876-143">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="8f876-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8f876-144">id</span><span class="sxs-lookup"><span data-stu-id="8f876-144">id</span></span> | <span data-ttu-id="8f876-145">String</span><span class="sxs-lookup"><span data-stu-id="8f876-145">String</span></span>| <span data-ttu-id="8f876-146">Уникальный идентификатор упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="8f876-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="8f876-147">котором</span><span class="sxs-lookup"><span data-stu-id="8f876-147">mentioned</span></span> | [<span data-ttu-id="8f876-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f876-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="8f876-149">Сведения электронной почты упомянутого человека.</span><span class="sxs-lookup"><span data-stu-id="8f876-149">The email information of the mentioned person.</span></span> <span data-ttu-id="8f876-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f876-150">Required.</span></span> |
|<span data-ttu-id="8f876-151">Ментионтекст</span><span class="sxs-lookup"><span data-stu-id="8f876-151">mentionText</span></span> | <span data-ttu-id="8f876-152">String</span><span class="sxs-lookup"><span data-stu-id="8f876-152">String</span></span> | <span data-ttu-id="8f876-153">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f876-153">Optional.</span></span> <span data-ttu-id="8f876-154">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="8f876-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="8f876-155">Чтобы получить упоминание в сообщении, ознакомьтесь со свойством **бодипревиев** этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="8f876-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="8f876-156">Серверкреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8f876-156">serverCreatedDateTime</span></span> | <span data-ttu-id="8f876-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f876-157">DateTimeOffset</span></span> | <span data-ttu-id="8f876-158">Дата и время создания упоминания на сервере.</span><span class="sxs-lookup"><span data-stu-id="8f876-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="8f876-159">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8f876-159">Optional.</span></span> <span data-ttu-id="8f876-160">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="8f876-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f876-161">Связи</span><span class="sxs-lookup"><span data-stu-id="8f876-161">Relationships</span></span>
<span data-ttu-id="8f876-162">Нет</span><span class="sxs-lookup"><span data-stu-id="8f876-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="8f876-163">Методы</span><span class="sxs-lookup"><span data-stu-id="8f876-163">Methods</span></span>

| <span data-ttu-id="8f876-164">Метод</span><span class="sxs-lookup"><span data-stu-id="8f876-164">Method</span></span>           | <span data-ttu-id="8f876-165">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f876-165">Return Type</span></span>    |<span data-ttu-id="8f876-166">Описание</span><span class="sxs-lookup"><span data-stu-id="8f876-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f876-167">[POST](../api/user-sendmail.md#request-2) и Send</span><span class="sxs-lookup"><span data-stu-id="8f876-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="8f876-168">Нет</span><span class="sxs-lookup"><span data-stu-id="8f876-168">None</span></span> | <span data-ttu-id="8f876-169">Создание и отправка упоминаний в виде части нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="8f876-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="8f876-170">[Публикация](../api/user-post-messages.md#request-2) в новом черновике</span><span class="sxs-lookup"><span data-stu-id="8f876-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="8f876-171">[сообщение](../resources/message.md) , которое содержит один или \*\*\*\* несколько объектов упоминаются.</span><span class="sxs-lookup"><span data-stu-id="8f876-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="8f876-172">Создайте черновик нового сообщения и добавьте в него один или несколько **упомянутых** объектов.</span><span class="sxs-lookup"><span data-stu-id="8f876-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="8f876-173">[Получение](../api/user-list-messages.md#request-2) сообщений с упоминанием меня</span><span class="sxs-lookup"><span data-stu-id="8f876-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="8f876-174">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="8f876-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="8f876-175">Получение всех сообщений в почтовом ящике вошедшего пользователя, который содержит **упоминание** этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="8f876-176">[Получение](../api/message-get.md#request-2) сообщения и его упоминаний</span><span class="sxs-lookup"><span data-stu-id="8f876-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="8f876-177">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="8f876-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="8f876-178">Получите сообщение и разверните сведения о каждом упоминании \*\*\*\* в сообщении.</span><span class="sxs-lookup"><span data-stu-id="8f876-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="8f876-179">[Удаление](../api/message-delete.md#request-2) упоминания</span><span class="sxs-lookup"><span data-stu-id="8f876-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="8f876-180">Нет</span><span class="sxs-lookup"><span data-stu-id="8f876-180">None</span></span> |<span data-ttu-id="8f876-181">Удаляет указанное упоминание из указанного сообщения в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f876-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
