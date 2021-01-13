---
title: Тип ресурса mention
description: Представляет уведомление для человека на основе его адреса электронной почты.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 23d4ac1d98a65e206a476768569cca89fb295a61
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844860"
---
# <a name="mention-resource-type"></a><span data-ttu-id="2915b-103">Тип ресурса mention</span><span class="sxs-lookup"><span data-stu-id="2915b-103">mention resource type</span></span>

<span data-ttu-id="2915b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2915b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2915b-105">Представляет уведомление для человека на основе его адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2915b-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="2915b-106">Этот тип уведомлений также называется @упоминаниями.</span><span class="sxs-lookup"><span data-stu-id="2915b-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="2915b-107">Ресурс [сообщения поддерживает](../resources/message.md) **упоминание.**</span><span class="sxs-lookup"><span data-stu-id="2915b-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="2915b-108">Он включает свойство **mentionsPreview,** которое указывает, упоминается ли во имя во включенного пользователя в этом экземпляре сообщения.</span><span class="sxs-lookup"><span data-stu-id="2915b-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="2915b-109">Он также включает свойство **навигации упоминаний,** которое поддерживает получение сведений об упоминаний или удаление упоминания в этом экземпляре.</span><span class="sxs-lookup"><span data-stu-id="2915b-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="2915b-110">При создании сообщения приложение может создать упоминание в том же запросе, включив упоминание в свойство `POST` **упоминаний.**</span><span class="sxs-lookup"><span data-stu-id="2915b-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="2915b-111">С помощью запроса с параметром запроса приложение может возвращать все сообщения в почтовом ящике пользователя, выписав `GET` `$filter` пользователя.</span><span class="sxs-lookup"><span data-stu-id="2915b-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="2915b-112">Запрос с параметром запроса позволяет приложению развернуть `GET` `$expand` все упоминания в определенном сообщении.</span><span class="sxs-lookup"><span data-stu-id="2915b-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="2915b-113">Этот механизм, позволяющий приложению устанавливать и получать упоминания в сообщениях, позволяет получать облегченные уведомления, когда пользователь, упоминающийся, может оставаться  в существующем контексте (например, при создании тела сообщения), а приложение задает свойство упоминаний.</span><span class="sxs-lookup"><span data-stu-id="2915b-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="2915b-114">Упомянутые лица могут легко узнать, упоминаются ли они в запросах с помощью параметра или `GET` `$filter` `$expand` параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="2915b-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="2915b-115">Например, в почтовом клиенте Outlook, когда пользователь вводит сообщение, Outlook позволяет пользователю выбрать или ввести имя для завершения `@` @упоминания.</span><span class="sxs-lookup"><span data-stu-id="2915b-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="2915b-116">Outlook задает свойство **упоминаний** перед созданием и отправкой сообщения или события.</span><span class="sxs-lookup"><span data-stu-id="2915b-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="2915b-117">Outlook также использует операции, с которыми во вписавшись пользователь может искать сообщения, в которых упоминается пользователь, оповещая пользователя о действиях или обсуждениях, что позволяет быстрее `GET` `$filter` `$expand` отвечать.</span><span class="sxs-lookup"><span data-stu-id="2915b-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2915b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2915b-118">JSON representation</span></span>

<span data-ttu-id="2915b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2915b-119">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2915b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="2915b-120">Properties</span></span>
| <span data-ttu-id="2915b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="2915b-121">Property</span></span>     | <span data-ttu-id="2915b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2915b-122">Type</span></span>   |<span data-ttu-id="2915b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2915b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2915b-124">application</span><span class="sxs-lookup"><span data-stu-id="2915b-124">application</span></span> | <span data-ttu-id="2915b-125">String</span><span class="sxs-lookup"><span data-stu-id="2915b-125">String</span></span> | <span data-ttu-id="2915b-126">Имя приложения, в котором создается упоминание.</span><span class="sxs-lookup"><span data-stu-id="2915b-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="2915b-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2915b-127">Optional.</span></span> <span data-ttu-id="2915b-128">Не используется и по умолчанию используется как значение null для **сообщения.**</span><span class="sxs-lookup"><span data-stu-id="2915b-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="2915b-129">clientReference</span><span class="sxs-lookup"><span data-stu-id="2915b-129">clientReference</span></span> | <span data-ttu-id="2915b-130">String</span><span class="sxs-lookup"><span data-stu-id="2915b-130">String</span></span> | <span data-ttu-id="2915b-131">Уникальный идентификатор, который представляет родительский экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="2915b-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="2915b-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2915b-132">Optional.</span></span> <span data-ttu-id="2915b-133">Не используется и по умолчанию используется как значение null для **сообщения.**</span><span class="sxs-lookup"><span data-stu-id="2915b-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="2915b-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="2915b-134">createdBy</span></span>  | [<span data-ttu-id="2915b-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2915b-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="2915b-136">Сведения по электронной почте пользователя, который сообщил об этом.</span><span class="sxs-lookup"><span data-stu-id="2915b-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="2915b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2915b-137">createdDateTime</span></span>  |<span data-ttu-id="2915b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2915b-138">DateTimeOffset</span></span> |<span data-ttu-id="2915b-139">Дата и время создания упоминания на клиенте.</span><span class="sxs-lookup"><span data-stu-id="2915b-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="2915b-140">deepLink</span><span class="sxs-lookup"><span data-stu-id="2915b-140">deepLink</span></span> | <span data-ttu-id="2915b-141">String</span><span class="sxs-lookup"><span data-stu-id="2915b-141">String</span></span> | <span data-ttu-id="2915b-142">Глубокая веб-ссылка на контекст упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="2915b-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="2915b-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2915b-143">Optional.</span></span> <span data-ttu-id="2915b-144">Не используется и по умолчанию используется как значение null для **сообщения.**</span><span class="sxs-lookup"><span data-stu-id="2915b-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="2915b-145">id</span><span class="sxs-lookup"><span data-stu-id="2915b-145">id</span></span> | <span data-ttu-id="2915b-146">String</span><span class="sxs-lookup"><span data-stu-id="2915b-146">String</span></span>| <span data-ttu-id="2915b-147">Уникальный идентификатор упоминания в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="2915b-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="2915b-148">упомянутый</span><span class="sxs-lookup"><span data-stu-id="2915b-148">mentioned</span></span> | [<span data-ttu-id="2915b-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2915b-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="2915b-150">Сведения по электронной почте упомянутого человека.</span><span class="sxs-lookup"><span data-stu-id="2915b-150">The email information of the mentioned person.</span></span> <span data-ttu-id="2915b-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2915b-151">Required.</span></span> |
|<span data-ttu-id="2915b-152">mentionText</span><span class="sxs-lookup"><span data-stu-id="2915b-152">mentionText</span></span> | <span data-ttu-id="2915b-153">String</span><span class="sxs-lookup"><span data-stu-id="2915b-153">String</span></span> | <span data-ttu-id="2915b-154">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2915b-154">Optional.</span></span> <span data-ttu-id="2915b-155">Не используется и по умолчанию используется как значение null для **сообщения.**</span><span class="sxs-lookup"><span data-stu-id="2915b-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="2915b-156">Чтобы получить упоминания в сообщении, см. свойство **bodyPreview** сообщения.</span><span class="sxs-lookup"><span data-stu-id="2915b-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="2915b-157">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2915b-157">serverCreatedDateTime</span></span> | <span data-ttu-id="2915b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2915b-158">DateTimeOffset</span></span> | <span data-ttu-id="2915b-159">Дата и время создания упоминания на сервере.</span><span class="sxs-lookup"><span data-stu-id="2915b-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="2915b-160">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2915b-160">Optional.</span></span> <span data-ttu-id="2915b-161">Не используется и по умолчанию используется как значение null для **сообщения.**</span><span class="sxs-lookup"><span data-stu-id="2915b-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2915b-162">Связи</span><span class="sxs-lookup"><span data-stu-id="2915b-162">Relationships</span></span>
<span data-ttu-id="2915b-163">Нет</span><span class="sxs-lookup"><span data-stu-id="2915b-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="2915b-164">Методы</span><span class="sxs-lookup"><span data-stu-id="2915b-164">Methods</span></span>

| <span data-ttu-id="2915b-165">Метод</span><span class="sxs-lookup"><span data-stu-id="2915b-165">Method</span></span>           | <span data-ttu-id="2915b-166">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2915b-166">Return Type</span></span>    |<span data-ttu-id="2915b-167">Описание</span><span class="sxs-lookup"><span data-stu-id="2915b-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2915b-168">[Публикация](../api/user-sendmail.md#request-2) и отправка</span><span class="sxs-lookup"><span data-stu-id="2915b-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="2915b-169">Нет</span><span class="sxs-lookup"><span data-stu-id="2915b-169">None</span></span> | <span data-ttu-id="2915b-170">Создание и отправка упоминаний в составе нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="2915b-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="2915b-171">[Публикация](../api/user-post-messages.md#request-2) в новом черновике</span><span class="sxs-lookup"><span data-stu-id="2915b-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="2915b-172">[сообщение,](../resources/message.md) которое содержит один или несколько **объектов упоминания.**</span><span class="sxs-lookup"><span data-stu-id="2915b-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="2915b-173">Создайте черновик нового сообщения и включив один или несколько объектов **упоминания.**</span><span class="sxs-lookup"><span data-stu-id="2915b-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="2915b-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span><span class="sxs-lookup"><span data-stu-id="2915b-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="2915b-175">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="2915b-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="2915b-176">Получите все сообщения в почтовом ящике во пользователя, во время которых есть упоминание **этого** пользователя.</span><span class="sxs-lookup"><span data-stu-id="2915b-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="2915b-177">[Получить](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) сообщение и его упоминания</span><span class="sxs-lookup"><span data-stu-id="2915b-177">[Get](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) a message and its mentions</span></span> | <span data-ttu-id="2915b-178">Коллекция [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="2915b-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="2915b-179">Получите сообщение и разберем подробности каждого **упоминания** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="2915b-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="2915b-180">[Удаление](../api/message-delete.md#request-2) упоминания</span><span class="sxs-lookup"><span data-stu-id="2915b-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="2915b-181">Нет</span><span class="sxs-lookup"><span data-stu-id="2915b-181">None</span></span> |<span data-ttu-id="2915b-182">Удаляет указанное упоминание в указанном сообщении в почтовом ящике пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="2915b-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

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


