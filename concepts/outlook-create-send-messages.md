---
title: Автоматизация создания, отправки и обработки сообщений
description: В Microsoft Graph электронные письма представлены ресурсом message.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b64c06d86cc4228a3254840103496dbe89890788
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474444"
---
# <a name="automate-creating-sending-and-processing-messages"></a><span data-ttu-id="68d4d-103">Автоматизация создания, отправки и обработки сообщений</span><span class="sxs-lookup"><span data-stu-id="68d4d-103">Automate creating, sending, and processing messages</span></span>

<span data-ttu-id="68d4d-104">В Microsoft Graph электронные письма представлены ресурсом [message](/graph/api/resources/message?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="68d4d-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="68d4d-105">По умолчанию сообщения можно идентифицировать по уникальному идентификатору записи в свойстве **id**.</span><span class="sxs-lookup"><span data-stu-id="68d4d-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="68d4d-106">При первоначальном создании и сохранении сообщения в качестве черновика или отправленного сообщения поставщик услуг хранилища назначает этому сообщению идентификатор записи.</span><span class="sxs-lookup"><span data-stu-id="68d4d-106">When a message is initially created and saved as a draft or sent, the store provider assigns the message an entry ID.</span></span> <span data-ttu-id="68d4d-107">По умолчанию этот идентификатор изменяется при копировании сообщения или его перемещении в другую папку, хранилище или PST-файл.</span><span class="sxs-lookup"><span data-stu-id="68d4d-107">By default, that ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span> <span data-ttu-id="68d4d-108">Для дальнейшей обработки сообщение указывается по текущему идентификатору.</span><span class="sxs-lookup"><span data-stu-id="68d4d-108">You reference the message by its current ID for further processing.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="68d4d-109">Создание и отправка почты</span><span class="sxs-lookup"><span data-stu-id="68d4d-109">Creating and sending mail</span></span>

<span data-ttu-id="68d4d-110">В Outlook вы можете создавать и отправлять электронные письма в одном и том же действии [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0). Вы также можете [создать](/graph/api/user-post-messages?view=graph-rest-1.0) черновик, затем [добавить содержимое](/graph/api/message-update?view=graph-rest-1.0) и [отправить](/graph/api/message-send?view=graph-rest-1.0) черновик.</span><span class="sxs-lookup"><span data-stu-id="68d4d-110">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="68d4d-111">Аналогично, при ответе на электронное письмо вы можете создавать и отправлять ответы в одном и том же действии ([ответить](/graph/api/message-reply?view=graph-rest-1.0), [ответить всем](/graph/api/message-replyall?view=graph-rest-1.0) или [переслать](/graph/api/message-forward?view=graph-rest-1.0)).</span><span class="sxs-lookup"><span data-stu-id="68d4d-111">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="68d4d-112">Кроме того, вы можете создать черновик для ответа ([ответить](/graph/api/message-createreply?view=graph-rest-1.0), [ответить всем](/graph/api/message-createreplyall?view=graph-rest-1.0) или [переслать](/graph/api/message-createforward?view=graph-rest-1.0)), [добавить содержимое](/graph/api/message-update?view=graph-rest-1.0), а затем [отправить ](/graph/api/message-send?view=graph-rest-1.0) черновик позже.</span><span class="sxs-lookup"><span data-stu-id="68d4d-112">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="68d4d-113">Чтобы программным способом отличать черновики от отправленных писем, проверяйте свойство **isDraft**.</span><span class="sxs-lookup"><span data-stu-id="68d4d-113">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="68d4d-114">По умолчанию черновики сообщений сохраняются в папке `Drafts`, а отправленные сообщения — в папке `Sent Items`.</span><span class="sxs-lookup"><span data-stu-id="68d4d-114">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="68d4d-115">Для удобства вы можете определить папки "Черновики" и "Отправленные", используя их [соответствующие хорошо известные имена папок](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="68d4d-115">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span>

### <a name="setting-the-from-and-sender-properties"></a><span data-ttu-id="68d4d-116">Задание свойств from и sender</span><span class="sxs-lookup"><span data-stu-id="68d4d-116">Setting the from and sender properties</span></span>

<span data-ttu-id="68d4d-117">В процессе создания сообщения в большинстве случаев Outlook указывает в качестве значения свойств **from** и **sender** одного и того же пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="68d4d-117">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="68d4d-118">Вы можете изменить эти свойства в указанных ниже ситуациях.</span><span class="sxs-lookup"><span data-stu-id="68d4d-118">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="68d4d-p105">Свойство **from** можно изменить, если администратор Exchange назначил другим пользователям права **sendAs** для почтового ящика. Для этого администратор может назначить его владельца, выбрав элемент **Разрешения для почтового ящика** на портале Azure, либо использовать Центр администрирования Exchange или командлет Add-ADPermission в Windows PowerShell. Затем программным способом можно задать свойство **from** одному из этих пользователей, обладающих правами **sendAs** для этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="68d4d-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="68d4d-122">Свойство **sender** можно изменить, если владелец почтового ящика предоставил одному или нескольким пользователям права на отправку сообщений из этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="68d4d-122">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="68d4d-123">Владелец почтового ящика может делегировать разрешения в Outlook.</span><span class="sxs-lookup"><span data-stu-id="68d4d-123">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="68d4d-124">Когда представитель отправляет сообщение от имени владельца почтового ящика, Outlook присваивает свойству **sender** учетную запись представителя, а в качестве значения свойства **from** остается владелец почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="68d4d-124">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="68d4d-125">Вы можете программным способом задать в качестве значения свойства **sender** пользователя, получившего разрешения представителя для этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="68d4d-125">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="68d4d-126">Проверка состояния получателя и экономия времени с помощью подсказок (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="68d4d-126">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="68d4d-127">С помощью [подсказок](/graph/api/resources/mailtips?view=graph-rest-beta) вы можете принимать обоснованные решения перед отправкой электронных писем.</span><span class="sxs-lookup"><span data-stu-id="68d4d-127">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="68d4d-128">Благодаря подсказкам можно получить ряд сведений, например о том, что почтовый ящик получателя доступен только для определенных отправителей, либо о том, что для отправки электронного письма получателю необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="68d4d-128">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>


## <a name="reading-messages-with-control-over-the-body-format-returned"></a><span data-ttu-id="68d4d-129">Чтение сообщений с управлением форматом возвращаемого текста</span><span class="sxs-lookup"><span data-stu-id="68d4d-129">Reading messages with control over the body format returned</span></span>

<span data-ttu-id="68d4d-130">Можно [прочитать сообщение](/graph/api/message-get?view=graph-rest-1.0) в почтовом ящике, указав его идентификатор:</span><span class="sxs-lookup"><span data-stu-id="68d4d-130">You can [read a message](/graph/api/message-get?view=graph-rest-1.0) in a mailbox by referencing its ID:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

Или можно [получать сообщения](/graph/api/user-list-messages?view=graph-rest-1.0) в определенной папке. <span data-ttu-id="68d4d-132">Например, чтобы читать сообщения в папке "Черновики" пользователя, вошедшего в систему, укажите следующее:</span><span class="sxs-lookup"><span data-stu-id="68d4d-132">For example, to read messages in the signed-in user's Drafts folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

<span data-ttu-id="68d4d-133">Текст сообщения Outlook может иметь либо формат HTML, либо текстовый формат. По умолчанию в отклике GET текст сообщения возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="68d4d-133">The body of an Outlook message can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="68d4d-134">При получении сообщения вы можете задать указанный ниже заголовок запроса, чтобы система возвратила свойства **body** и **uniqueBody** в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="68d4d-134">When getting a message, you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="68d4d-135">Чтобы получить текст сообщения в формате HTML, задайте указанный ниже заголовок или просто пропустите его.</span><span class="sxs-lookup"><span data-stu-id="68d4d-135">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="68d4d-136">Когда вы указываете какой-либо заголовок, успешный отклик будет включать соответствующий заголовок `Preference-Applied`.</span><span class="sxs-lookup"><span data-stu-id="68d4d-136">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="68d4d-137">Чтобы получить результат выполнения запроса в текстовом формате: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="68d4d-137">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="68d4d-138">Чтобы получить результат выполнения запроса в формате HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="68d4d-138">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="68d4d-139">Если текст сообщения имеет формат HTML, то по умолчанию прежде чем возвратить текст сообщения в отклике REST, Outlook удаляет весь потенциально небезопасный HTML-код (например, код JavaScript), внедренный в свойство **body**.</span><span class="sxs-lookup"><span data-stu-id="68d4d-139">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="68d4d-140">Чтобы получить все исходное содержимое в формате HTML, добавьте следующий заголовок HTTP-запроса:</span><span class="sxs-lookup"><span data-stu-id="68d4d-140">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="68d4d-141">Интеграция с социальными жестами (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="68d4d-141">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="68d4d-142">@Упоминания — это уведомления для пользователей, о том, что их упомянули в сообщениях.</span><span class="sxs-lookup"><span data-stu-id="68d4d-142">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="68d4d-143">С помощью ресурса [mention](/graph/api/resources/mention?view=graph-rest-beta) приложения могут задавать и получать стандартный социальный жест в Интернете (префикс @) в письмах.</span><span class="sxs-lookup"><span data-stu-id="68d4d-143">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="68d4d-144">Вы можете выполнить указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="68d4d-144">You can:</span></span>

- <span data-ttu-id="68d4d-145">Создавать @упоминания при [составлении сообщений](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span><span class="sxs-lookup"><span data-stu-id="68d4d-145">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="68d4d-146">Получать все сообщения в почтовом ящике пользователя, содержащие @упоминание пользователя</span><span class="sxs-lookup"><span data-stu-id="68d4d-146">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="68d4d-147">Получать все @упоминания в сообщении</span><span class="sxs-lookup"><span data-stu-id="68d4d-147">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="68d4d-148">Другие общие возможности</span><span class="sxs-lookup"><span data-stu-id="68d4d-148">Other shared capabilities</span></span>

<span data-ttu-id="68d4d-149">Используйте указанные ниже стандартные возможности, имеющиеся в объектах Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="68d4d-149">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="68d4d-150">Вы можете подписаться на [уведомления об изменениях](/graph/api/resources/webhooks?view=graph-rest-1.0) сообщений. Вы будете получать их при возникновении изменений одного или нескольких типов, например при создании или изменении сообщений.</span><span class="sxs-lookup"><span data-stu-id="68d4d-150">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="68d4d-151">[Вы можете отслеживать эти добавочные изменения сообщений в папке](delta-query-messages.md).</span><span class="sxs-lookup"><span data-stu-id="68d4d-151">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="68d4d-152">Вы можете создавать [открытые расширения](extensibility-overview.md#open-extensions) или [расширения схемы](extensibility-overview.md#schema-extensions), чтобы добавлять пользовательские данные в экземпляры сообщений.</span><span class="sxs-lookup"><span data-stu-id="68d4d-152">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="68d4d-153">Вы можете создавать [расширенные свойства](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) в экземплярах сообщений, чтобы хранить пользовательские данные для свойств MAPI Outlook, когда эти свойства еще недоступны в метаданных API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="68d4d-153">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="68d4d-154">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="68d4d-154">Next steps</span></span>

<span data-ttu-id="68d4d-155">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="68d4d-155">Find out more about:</span></span>

- [<span data-ttu-id="68d4d-156">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="68d4d-156">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- [<span data-ttu-id="68d4d-157">Получение содержимого MIME (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="68d4d-157">Get MIME content (preview)</span></span>](outlook-get-mime-message.md)
- [<span data-ttu-id="68d4d-158">Получение общих сообщений</span><span class="sxs-lookup"><span data-stu-id="68d4d-158">Get shared messages</span></span>](outlook-share-messages-folders.md)
- [<span data-ttu-id="68d4d-159">Отправка сообщений Outlook от другого пользователя</span><span class="sxs-lookup"><span data-stu-id="68d4d-159">Send Outlook messages from another user</span></span>](outlook-send-mail-from-other-user.md)
- [<span data-ttu-id="68d4d-160">Получение неизменяемых идентификаторов для ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="68d4d-160">Get immutable identifiers for Outlook resources</span></span>](outlook-immutable-id.md)
- <span data-ttu-id="68d4d-161">[Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [варианты использования](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="68d4d-161">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
