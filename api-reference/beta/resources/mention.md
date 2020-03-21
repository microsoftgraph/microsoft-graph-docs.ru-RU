---
title: Тип ресурса "упоминание"
description: Представляет уведомление для пользователя на основе электронного адреса пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 70005abbe8eaf0e9680f106f59caf091aa2495d2
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892585"
---
# <a name="mention-resource-type"></a><span data-ttu-id="67522-103">Тип ресурса "упоминание"</span><span class="sxs-lookup"><span data-stu-id="67522-103">mention resource type</span></span>

<span data-ttu-id="67522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67522-105">Представляет уведомление для пользователя на основе электронного адреса пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="67522-106">Этот тип уведомления также называется @-упоминаниями.</span><span class="sxs-lookup"><span data-stu-id="67522-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="67522-107">Ресурс [Message](../resources/message.md) поддерживает **упоминание**.</span><span class="sxs-lookup"><span data-stu-id="67522-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="67522-108">Он включает свойство **ментионспревиев** , которое указывает, упоминается ли вошедшего в данный экземпляр сообщения пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="67522-109">Кроме того, он включает свойство навигации **упоминаютй** , которое поддерживает сбор сведений о упоминании или удаление упоминания в этом экземпляре.</span><span class="sxs-lookup"><span data-stu-id="67522-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="67522-110">При создании сообщения приложение может создать упоминание в том же `POST` запросе, включив в свойство **упоминаются** упоминание.</span><span class="sxs-lookup"><span data-stu-id="67522-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="67522-111">С помощью `GET` запроса с параметром `$filter` Query приложение может возвратить все сообщения в почтовом ящике вошедшего пользователя, который упоминает пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="67522-112">`GET` Запрос с параметром `$expand` запроса позволяет приложению развернуть все упоминания в определенном сообщении.</span><span class="sxs-lookup"><span data-stu-id="67522-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="67522-113">Этот механизм, позволяющий приложениям устанавливать и получать упоминания в сообщениях, включает облегченные уведомления, где пользователь, проверяя упоминание, может находиться в существующем контексте (например, составление текста сообщения), пока приложение устанавливает базовое свойство **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="67522-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="67522-114">Упомянутые лица могут легко выяснить, где они упоминаются с помощью `GET` запросов с `$filter` параметром `$expand` или с помощью параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="67522-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="67522-115">Например, в почтовом клиенте Outlook, когда пользователь вводит `@` сообщение, Outlook позволяет пользователю выбрать или ввести имя для завершения @ – упоминаний.</span><span class="sxs-lookup"><span data-stu-id="67522-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="67522-116">Outlook задает свойство **упоминаются** перед созданием и отправкой сообщения или события.</span><span class="sxs-lookup"><span data-stu-id="67522-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="67522-117">Outlook также использует `GET` операции с `$filter` и `$expand` , чтобы пользователь, вошедшего в систему, мог выполнять поиск сообщений, которые упоминают пользователя, предупреждает пользователя о действиях или обсуждениях, что позволяет быстрее отреагировать на действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="67522-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67522-118">JSON representation</span></span>

<span data-ttu-id="67522-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67522-119">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="67522-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="67522-120">Properties</span></span>
| <span data-ttu-id="67522-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="67522-121">Property</span></span>     | <span data-ttu-id="67522-122">Тип</span><span class="sxs-lookup"><span data-stu-id="67522-122">Type</span></span>   |<span data-ttu-id="67522-123">Описание</span><span class="sxs-lookup"><span data-stu-id="67522-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67522-124">application</span><span class="sxs-lookup"><span data-stu-id="67522-124">application</span></span> | <span data-ttu-id="67522-125">String</span><span class="sxs-lookup"><span data-stu-id="67522-125">String</span></span> | <span data-ttu-id="67522-126">Имя приложения, в котором создается упоминание.</span><span class="sxs-lookup"><span data-stu-id="67522-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="67522-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="67522-127">Optional.</span></span> <span data-ttu-id="67522-128">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="67522-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="67522-129">клиентреференце</span><span class="sxs-lookup"><span data-stu-id="67522-129">clientReference</span></span> | <span data-ttu-id="67522-130">String</span><span class="sxs-lookup"><span data-stu-id="67522-130">String</span></span> | <span data-ttu-id="67522-131">Уникальный идентификатор, представляющий родительский объект для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="67522-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="67522-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="67522-132">Optional.</span></span> <span data-ttu-id="67522-133">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="67522-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="67522-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="67522-134">createdBy</span></span>  | [<span data-ttu-id="67522-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="67522-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="67522-136">Сведения электронной почты пользователя, выполнившего упоминание.</span><span class="sxs-lookup"><span data-stu-id="67522-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="67522-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67522-137">createdDateTime</span></span>  |<span data-ttu-id="67522-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67522-138">DateTimeOffset</span></span> |<span data-ttu-id="67522-139">Дата и время создания упоминания в клиенте.</span><span class="sxs-lookup"><span data-stu-id="67522-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="67522-140">Прямой</span><span class="sxs-lookup"><span data-stu-id="67522-140">deepLink</span></span> | <span data-ttu-id="67522-141">String</span><span class="sxs-lookup"><span data-stu-id="67522-141">String</span></span> | <span data-ttu-id="67522-142">Глубокая веб-ссылка на контекст упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="67522-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="67522-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="67522-143">Optional.</span></span> <span data-ttu-id="67522-144">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="67522-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="67522-145">id</span><span class="sxs-lookup"><span data-stu-id="67522-145">id</span></span> | <span data-ttu-id="67522-146">String</span><span class="sxs-lookup"><span data-stu-id="67522-146">String</span></span>| <span data-ttu-id="67522-147">Уникальный идентификатор упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="67522-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="67522-148">котором</span><span class="sxs-lookup"><span data-stu-id="67522-148">mentioned</span></span> | [<span data-ttu-id="67522-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="67522-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="67522-150">Сведения электронной почты упомянутого человека.</span><span class="sxs-lookup"><span data-stu-id="67522-150">The email information of the mentioned person.</span></span> <span data-ttu-id="67522-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67522-151">Required.</span></span> |
|<span data-ttu-id="67522-152">ментионтекст</span><span class="sxs-lookup"><span data-stu-id="67522-152">mentionText</span></span> | <span data-ttu-id="67522-153">String</span><span class="sxs-lookup"><span data-stu-id="67522-153">String</span></span> | <span data-ttu-id="67522-154">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="67522-154">Optional.</span></span> <span data-ttu-id="67522-155">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="67522-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="67522-156">Чтобы получить упоминание в сообщении, ознакомьтесь со свойством **бодипревиев** этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="67522-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="67522-157">серверкреатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="67522-157">serverCreatedDateTime</span></span> | <span data-ttu-id="67522-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67522-158">DateTimeOffset</span></span> | <span data-ttu-id="67522-159">Дата и время создания упоминания на сервере.</span><span class="sxs-lookup"><span data-stu-id="67522-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="67522-160">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="67522-160">Optional.</span></span> <span data-ttu-id="67522-161">Не используется и по умолчанию задано значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="67522-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="67522-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="67522-162">Relationships</span></span>
<span data-ttu-id="67522-163">Нет</span><span class="sxs-lookup"><span data-stu-id="67522-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="67522-164">Методы</span><span class="sxs-lookup"><span data-stu-id="67522-164">Methods</span></span>

| <span data-ttu-id="67522-165">Метод</span><span class="sxs-lookup"><span data-stu-id="67522-165">Method</span></span>           | <span data-ttu-id="67522-166">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="67522-166">Return Type</span></span>    |<span data-ttu-id="67522-167">Описание</span><span class="sxs-lookup"><span data-stu-id="67522-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67522-168">[POST](../api/user-sendmail.md#request-2) и Send</span><span class="sxs-lookup"><span data-stu-id="67522-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="67522-169">Нет</span><span class="sxs-lookup"><span data-stu-id="67522-169">None</span></span> | <span data-ttu-id="67522-170">Создание и отправка упоминаний в виде части нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="67522-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="67522-171">[Публикация](../api/user-post-messages.md#request-2) в новом черновике</span><span class="sxs-lookup"><span data-stu-id="67522-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="67522-172">[сообщение](../resources/message.md) , которое содержит один или несколько объектов **упоминаются** .</span><span class="sxs-lookup"><span data-stu-id="67522-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="67522-173">Создайте черновик нового сообщения и добавьте в него один или несколько **упомянутых** объектов.</span><span class="sxs-lookup"><span data-stu-id="67522-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="67522-174">[Получение](../api/user-list-messages.md#request-2) сообщений с упоминанием меня</span><span class="sxs-lookup"><span data-stu-id="67522-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="67522-175">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="67522-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="67522-176">Получение всех сообщений в почтовом ящике вошедшего пользователя, который содержит **упоминание** этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="67522-177">[Получение](../api/message-get.md#example-2) сообщения и его упоминаний</span><span class="sxs-lookup"><span data-stu-id="67522-177">[Get](../api/message-get.md#example-2) a message and its mentions</span></span> | <span data-ttu-id="67522-178">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="67522-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="67522-179">Получите сообщение и разверните сведения о каждом **упоминании** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="67522-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="67522-180">[Удаление](../api/message-delete.md#request-2) упоминания</span><span class="sxs-lookup"><span data-stu-id="67522-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="67522-181">Нет</span><span class="sxs-lookup"><span data-stu-id="67522-181">None</span></span> |<span data-ttu-id="67522-182">Удаляет указанное упоминание из указанного сообщения в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="67522-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

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
