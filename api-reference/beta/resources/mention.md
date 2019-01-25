---
title: Укажите тип ресурса
description: Представляет уведомления для пользователя, на основе адреса электронной почты контакта.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523199"
---
# <a name="mention-resource-type"></a><span data-ttu-id="3206d-103">Укажите тип ресурса</span><span class="sxs-lookup"><span data-stu-id="3206d-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3206d-104">Представляет уведомления для пользователя, на основе адреса электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="3206d-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="3206d-105">Этот тип уведомления также называется @ упоминания.</span><span class="sxs-lookup"><span data-stu-id="3206d-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="3206d-106">Ресурс [сообщений](../resources/message.md) поддерживает **упомянуть**.</span><span class="sxs-lookup"><span data-stu-id="3206d-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="3206d-107">Он содержит свойство **mentionsPreview** , которое указывает, описанного ли пользователь выполнил вход в этот экземпляр сообщения.</span><span class="sxs-lookup"><span data-stu-id="3206d-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="3206d-108">Он также включает свойство навигации **упоминания** , которое поддерживает получение сведений о Упоминание или удаление упоминаются в этот экземпляр.</span><span class="sxs-lookup"><span data-stu-id="3206d-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="3206d-109">При создании сообщения, приложение можно создать упоминаются в том же `POST` запрос, включая упоминаются в свойстве **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="3206d-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="3206d-110">С помощью `GET` запрос с `$filter` параметр запроса, приложение может вернуть все сообщения в почтовом ящике пользователь выполнил вход, упомянуть пользователя.</span><span class="sxs-lookup"><span data-stu-id="3206d-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="3206d-111">A `GET` запрос с `$expand` параметр позволяет приложение разверните все упоминания в определенное сообщение запроса.</span><span class="sxs-lookup"><span data-stu-id="3206d-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="3206d-112">Этот механизм, позволяющий приложения задание и извлечение упоминания в сообщениях на включает lightweight уведомления, где пользователя, выполняющего упоминание могут оставаться в существующий контекст (например, при составлении сообщения) при приложение задает свойство базового **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="3206d-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="3206d-113">Упомянутые лиц можно легко выяснить, если и где упомянутые через `GET` запрашивает с `$filter` или `$expand` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="3206d-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="3206d-114">Например, в почтовом клиенте Outlook, когда пользователь вводит `@` при записи сообщения Outlook позволяет пользователей выберите или введите имя для выполнения упоминание @.</span><span class="sxs-lookup"><span data-stu-id="3206d-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="3206d-115">Outlook устанавливает для свойства **упоминания** перед создает и отправляет сообщение или события.</span><span class="sxs-lookup"><span data-stu-id="3206d-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="3206d-116">Outlook также использует `GET` операции с `$filter` и `$expand` сообщите пользователь выполнил вход искать сообщения, содержащие упоминание пользователя, элемент интерфейса, предупреждающий пользователя элементы действия или обсуждения, что обеспечивает более быстрый отклик.</span><span class="sxs-lookup"><span data-stu-id="3206d-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3206d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3206d-117">JSON representation</span></span>

<span data-ttu-id="3206d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3206d-118">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3206d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3206d-119">Properties</span></span>
| <span data-ttu-id="3206d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3206d-120">Property</span></span>     | <span data-ttu-id="3206d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3206d-121">Type</span></span>   |<span data-ttu-id="3206d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3206d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3206d-123">application</span><span class="sxs-lookup"><span data-stu-id="3206d-123">application</span></span> | <span data-ttu-id="3206d-124">String</span><span class="sxs-lookup"><span data-stu-id="3206d-124">String</span></span> | <span data-ttu-id="3206d-125">Имя приложения, где создается упоминание.</span><span class="sxs-lookup"><span data-stu-id="3206d-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="3206d-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3206d-126">Optional.</span></span> <span data-ttu-id="3206d-127">Не используется и не по умолчанию установлено значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3206d-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3206d-128">clientReference</span><span class="sxs-lookup"><span data-stu-id="3206d-128">clientReference</span></span> | <span data-ttu-id="3206d-129">String</span><span class="sxs-lookup"><span data-stu-id="3206d-129">String</span></span> | <span data-ttu-id="3206d-130">Уникальный идентификатор, представляющий родительский объект экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="3206d-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="3206d-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3206d-131">Optional.</span></span> <span data-ttu-id="3206d-132">Не используется и не по умолчанию установлено значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3206d-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3206d-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="3206d-133">createdBy</span></span>  | [<span data-ttu-id="3206d-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3206d-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="3206d-135">Сведения о электронной почты пользователя, выполнившего упоминание.</span><span class="sxs-lookup"><span data-stu-id="3206d-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="3206d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3206d-136">createdDateTime</span></span>  |<span data-ttu-id="3206d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3206d-137">DateTimeOffset</span></span> |<span data-ttu-id="3206d-138">Дата и время создания упоминаются в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3206d-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="3206d-139">deepLink</span><span class="sxs-lookup"><span data-stu-id="3206d-139">deepLink</span></span> | <span data-ttu-id="3206d-140">String</span><span class="sxs-lookup"><span data-stu-id="3206d-140">String</span></span> | <span data-ttu-id="3206d-141">Глубокое web ссылка на контексте упоминаются в экземпляре ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3206d-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="3206d-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3206d-142">Optional.</span></span> <span data-ttu-id="3206d-143">Не используется и не по умолчанию установлено значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3206d-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="3206d-144">id</span><span class="sxs-lookup"><span data-stu-id="3206d-144">id</span></span> | <span data-ttu-id="3206d-145">String</span><span class="sxs-lookup"><span data-stu-id="3206d-145">String</span></span>| <span data-ttu-id="3206d-146">Уникальный идентификатор упоминаются в экземпляре ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3206d-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="3206d-147">упомянутые</span><span class="sxs-lookup"><span data-stu-id="3206d-147">mentioned</span></span> | [<span data-ttu-id="3206d-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3206d-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="3206d-149">Сведения о электронной почты человека, упомянутых выше.</span><span class="sxs-lookup"><span data-stu-id="3206d-149">The email information of the mentioned person.</span></span> <span data-ttu-id="3206d-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3206d-150">Required.</span></span> |
|<span data-ttu-id="3206d-151">mentionText</span><span class="sxs-lookup"><span data-stu-id="3206d-151">mentionText</span></span> | <span data-ttu-id="3206d-152">String</span><span class="sxs-lookup"><span data-stu-id="3206d-152">String</span></span> | <span data-ttu-id="3206d-153">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3206d-153">Optional.</span></span> <span data-ttu-id="3206d-154">Не используется и не по умолчанию установлено значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3206d-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="3206d-155">Чтобы получить упоминания в сообщении, см **bodyPreview** сообщения вместо этого.</span><span class="sxs-lookup"><span data-stu-id="3206d-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="3206d-156">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3206d-156">serverCreatedDateTime</span></span> | <span data-ttu-id="3206d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3206d-157">DateTimeOffset</span></span> | <span data-ttu-id="3206d-158">Дата и время создания упоминание на сервере.</span><span class="sxs-lookup"><span data-stu-id="3206d-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="3206d-159">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3206d-159">Optional.</span></span> <span data-ttu-id="3206d-160">Не используется и не по умолчанию установлено значение NULL для **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3206d-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3206d-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="3206d-161">Relationships</span></span>
<span data-ttu-id="3206d-162">Нет</span><span class="sxs-lookup"><span data-stu-id="3206d-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="3206d-163">Методы</span><span class="sxs-lookup"><span data-stu-id="3206d-163">Methods</span></span>

| <span data-ttu-id="3206d-164">Метод</span><span class="sxs-lookup"><span data-stu-id="3206d-164">Method</span></span>           | <span data-ttu-id="3206d-165">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3206d-165">Return Type</span></span>    |<span data-ttu-id="3206d-166">Описание</span><span class="sxs-lookup"><span data-stu-id="3206d-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3206d-167">[Учет](../api/user-sendmail.md#request-2) и отправки</span><span class="sxs-lookup"><span data-stu-id="3206d-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="3206d-168">Нет</span><span class="sxs-lookup"><span data-stu-id="3206d-168">None</span></span> | <span data-ttu-id="3206d-169">Создание и отправка упоминания как часть нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="3206d-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="3206d-170">[Публикация в](../api/user-post-messages.md#request-2) новый черновик</span><span class="sxs-lookup"><span data-stu-id="3206d-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="3206d-171">[сообщение](../resources/message.md) , которое содержит один или несколько объектов **упомянуть** .</span><span class="sxs-lookup"><span data-stu-id="3206d-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="3206d-172">Создайте проект новое сообщение и включать один или несколько объектов **упомянуть** .</span><span class="sxs-lookup"><span data-stu-id="3206d-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="3206d-173">[Получение](../api/user-list-messages.md#request-2) сообщений упоминание обо мне</span><span class="sxs-lookup"><span data-stu-id="3206d-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="3206d-174">Коллекция объектов [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="3206d-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="3206d-175">Получение всех сообщений в почтовый ящик пользователя выполнил вход, содержащие **упомянуть** о этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="3206d-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="3206d-176">[Получите](../api/message-get.md#request-2) сообщение и его упоминания</span><span class="sxs-lookup"><span data-stu-id="3206d-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="3206d-177">Коллекция объектов [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="3206d-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="3206d-178">Появится сообщение, а затем разверните сведения о каждом **упомянуть** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="3206d-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="3206d-179">[Удаление](../api/message-delete.md#request-2) упоминание</span><span class="sxs-lookup"><span data-stu-id="3206d-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="3206d-180">Нет</span><span class="sxs-lookup"><span data-stu-id="3206d-180">None</span></span> |<span data-ttu-id="3206d-181">Удаляет указанный упоминаются в указанное сообщение в почтовый ящик пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3206d-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
