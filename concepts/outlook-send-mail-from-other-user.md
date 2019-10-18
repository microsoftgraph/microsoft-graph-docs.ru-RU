---
title: Отправка сообщений Outlook от другого пользователя
description: Используйте разрешения "Отправить как" и "Отправить от имени" для отправки сообщений Outlook от другого пользователя или с общего почтового ящика в Microsoft Graph.
author: jasonjoh
localization_priority: Priority
ms.prod: outlook
ms.date: 01/16/2019
ms.openlocfilehash: 03cfa3d532b2eb0494cc220c1c315b14bd9652c1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735097"
---
# <a name="send-outlook-messages-from-another-user"></a><span data-ttu-id="f72ac-103">Отправка сообщений Outlook от другого пользователя</span><span class="sxs-lookup"><span data-stu-id="f72ac-103">Send Outlook messages from another user</span></span>

<span data-ttu-id="f72ac-104">Exchange Online предусматривает [разрешения для почтового ящика](/Exchange/recipients/mailbox-permissions), позволяющие пользователю отправлять электронную почту таким образом, чтобы в качестве отправителя значился другой пользователь, список рассылки, группа, ресурс или общий почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="f72ac-104">Exchange Online provides [mailbox permissions](/Exchange/recipients/mailbox-permissions) that allow a user to send mail that appears to be sent from another user, distribution list, group, resource, or shared mailbox.</span></span> <span data-ttu-id="f72ac-105">Microsoft Graph также поддерживает эту функцию, но конечный результат может отличаться в зависимости от точных разрешений, предоставленных в Exchange Online, а также того, какие API были использованы для отправки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f72ac-105">Microsoft Graph supports this feature as well, but the end result varies depending on the exact permissions granted in Exchange Online and which API you use to send the mail.</span></span>

## <a name="permissions"></a><span data-ttu-id="f72ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f72ac-106">Permissions</span></span>

<span data-ttu-id="f72ac-107">К сообщениям, отправляемым от другого пользователя, применяются два типа разрешений: [разрешения Microsoft Graph](permissions-reference.md) и разрешения для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f72ac-107">Two types of permissions apply to sending messages from another user: [Microsoft Graph permissions](permissions-reference.md), and mailbox permissions.</span></span>

### <a name="microsoft-graph-permissions"></a><span data-ttu-id="f72ac-108">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f72ac-108">Microsoft Graph permissions</span></span>

<span data-ttu-id="f72ac-109">Чтобы отправлять сообщения от другого пользователя, приложения, использующие маркеры пользователя, используют разрешение **Mail.Send.Shared**.</span><span class="sxs-lookup"><span data-stu-id="f72ac-109">In order to send messages from another user, applications that use user tokens use the **Mail.Send.Shared** permission.</span></span>

> [!NOTE]
> <span data-ttu-id="f72ac-110">Приложения, использующие маркеры приложения вместо маркеров пользователя и имеющие разрешение **Mail.Send**, предоставленное администратором, могут отправлять почту как любой пользователь в организации, отправляя сообщение в обычном порядке с почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="f72ac-110">Applications that use application tokens instead of user tokens and have the **Mail.Send** permission consented by an administrator can send mail as any user in the organization by sending the mail normally through the user's mailbox.</span></span>

### <a name="mailbox-permissions"></a><span data-ttu-id="f72ac-111">Разрешения для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="f72ac-111">Mailbox permissions</span></span>

<span data-ttu-id="f72ac-112">На конечный результат отправки сообщения от другого пользователя влияют два разрешения: **Отправить от имени** и **Отправить как**.</span><span class="sxs-lookup"><span data-stu-id="f72ac-112">Two permissions affect the end result of sending a message from another user: **Send on Behalf** and **Send As**.</span></span> <span data-ttu-id="f72ac-113">Пользователь, который выполнил вход в приложение, используя разрешение **Mail.Send.Shared**, ДОЛЖЕН иметь по крайней мере одно из таких разрешений, предоставленных для почтового ящика, группы или списка рассылки, которые значатся в качестве отправителя.</span><span class="sxs-lookup"><span data-stu-id="f72ac-113">The user that is signed in to your application with the **Mail.Send.Shared** permission MUST have at least one of these permissions granted to the mailbox, group, or distribution list that the mail is from.</span></span>

#### <a name="send-on-behalf"></a><span data-ttu-id="f72ac-114">Отправить от имени</span><span class="sxs-lookup"><span data-stu-id="f72ac-114">Send on Behalf</span></span>

<span data-ttu-id="f72ac-115">С таким разрешением получатель почты получает указание в почтовом клиенте, что сообщение было отправлено пользователем приложения от имени другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f72ac-115">With this permission, the recipient of the email has an indication in their email client that the message was sent by the user of your application on behalf of another user.</span></span>

![Снимок экрана Outlook в Интернете с указанием того, что сообщение было отправлено одним пользователям от имени другого](images/outlook-sent-on-behalf.png)

<span data-ttu-id="f72ac-117">В Microsoft Graph это представлено в виде свойств `sender` (пользователь, который фактически отправил сообщение) и `from` (пользователь, группа или другое, отображаемые в качестве отправителя).</span><span class="sxs-lookup"><span data-stu-id="f72ac-117">This is exposed in Microsoft Graph as the `sender` (user that actually sent the message) and `from` (user/group/etc. that the message appears to be from) properties.</span></span>

```json
{
  "id": "AAMkAGE1...",
  "subject": "Send mail test",
  "sender": {
    "emailAddress": {
      "name": "Adele Vance",
      "address": "AdeleV@contoso.com"
    }
  },
  "from": {
    "emailAddress": {
      "name": "Pradeep Gupta",
      "address": "PradeepG@contoso.com"
    }
  }
}
```

<span data-ttu-id="f72ac-118">Пользователь может предоставлять это разрешение для своего почтового ящика другому пользователю, [используя Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span><span class="sxs-lookup"><span data-stu-id="f72ac-118">A user can grant this permission for their own mailbox to another user by [using Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span></span> <span data-ttu-id="f72ac-119">Администраторы могут предоставить это разрешение для любого почтового ящика, группы или списка рассылки в [Центре администрирования Office 365](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f72ac-119">Administrators can grant this permission for any mailbox, group, or distribution list in the [Office 365 admin center](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span></span>

#### <a name="send-as"></a><span data-ttu-id="f72ac-120">Отправить как</span><span class="sxs-lookup"><span data-stu-id="f72ac-120">Send As</span></span>

<span data-ttu-id="f72ac-121">С таким разрешением нет указаний относительного того, что сообщение было отправлено от другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f72ac-121">With this permission, there is no indication that the message was sent as a different user.</span></span> <span data-ttu-id="f72ac-122">Свойства `sender` и `from` имеют одинаковое значение.</span><span class="sxs-lookup"><span data-stu-id="f72ac-122">The `sender` and `from` properties have the same value.</span></span>

<span data-ttu-id="f72ac-123">Пользователи не могут предоставить это разрешение своим почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="f72ac-123">Users cannot grant this permission to their mailboxes.</span></span> <span data-ttu-id="f72ac-124">Администраторы могут предоставлять это разрешение в Центре администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="f72ac-124">Admins can grant this permission in the Office 365 admin center.</span></span>

## <a name="sending-with-microsoft-graph"></a><span data-ttu-id="f72ac-125">Отправка с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f72ac-125">Sending with Microsoft Graph</span></span>

<span data-ttu-id="f72ac-126">Вы можете отправлять сообщения от другого пользователя, [отправляя их напрямую](/graph/api/user-sendmail?view=graph-rest-1.0) либо [создавая черновик](/graph/api/user-post-messages?view=graph-rest-1.0), а затем [отправляя его](/graph/api/message-send?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f72ac-126">You can send messages from another user by either [sending directly](/graph/api/user-sendmail?view=graph-rest-1.0) or by [creating a draft](/graph/api/user-post-messages?view=graph-rest-1.0) and then [sending it](/graph/api/message-send?view=graph-rest-1.0).</span></span>

<span data-ttu-id="f72ac-127">Чтобы отправлять сообщения от другого пользователя, задайте свойство `from` в [сообщении](/graph/api/resources/message?view=graph-rest-1.0), отправляемом на адрес электронной почты пользователя, который должен значиться в качестве отправителя.</span><span class="sxs-lookup"><span data-stu-id="f72ac-127">In order to send from another user, set the `from` property on the [message](/graph/api/resources/message?view=graph-rest-1.0) sent to the email address of the user to send from.</span></span> <span data-ttu-id="f72ac-128">Вам не нужно задавать свойство `sender` — Microsoft Graph задаст его надлежащим образом, на основе разрешений почтового ящика, предоставленных пользователю, который выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="f72ac-128">You don't need to set the `sender` property - Microsoft Graph will set it appropriately, based on the mailbox permissions granted to the user who has signed in.</span></span>

<span data-ttu-id="f72ac-129">Например, для отправки электронной почты от группы `sales@contoso.com` задайте настройки сообщения как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="f72ac-129">For example, to send mail from the `sales@contoso.com` group, configure the message as follows.</span></span>

```json
{
  "subject": "January sales report",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "MeganB@contoso.com"
      }
    }
  ],
  "from": {
    "emailAddress": {
      "address": "sales@contoso.com"
    }
  }
}
```

## <a name="sent-items-behavior"></a><span data-ttu-id="f72ac-130">Порядок сохранения в папке "Отправленные"</span><span class="sxs-lookup"><span data-stu-id="f72ac-130">Sent Items behavior</span></span>

<span data-ttu-id="f72ac-131">После отправки сообщения его можно сохранить в папке "Отправленные" фактического отправителя, в папке "Отправленные" пользователя, который значится как отправитель, или в обеих папках.</span><span class="sxs-lookup"><span data-stu-id="f72ac-131">After the message is sent, it can be saved to the sending user's Sent Items folder, the from user's Sent Items folder, or both.</span></span> <span data-ttu-id="f72ac-132">Его также можно не сохранять.</span><span class="sxs-lookup"><span data-stu-id="f72ac-132">It can also not be saved at all.</span></span>

> [!NOTE]
> <span data-ttu-id="f72ac-133">Если сообщение будет отправлено с адреса, который не имеет почтового ящика (например, список рассылки), папки "Отправленные" у пользователя, значащегося в качестве отправителя, нет.</span><span class="sxs-lookup"><span data-stu-id="f72ac-133">If the message is sent from an address that does not have a mailbox (a distribution list, for example), there is no Sent Items for the from user.</span></span>

- <span data-ttu-id="f72ac-134">Если ваше приложение выполняет отправку с использованием конечной точки `/me` (или `/users/{user-id}`, где `user-id` соответствует пользователю, который выполнил вход), по умолчанию сообщение будет сохранено в папке "Отправленные" пользователя, являющегося отправителем.</span><span class="sxs-lookup"><span data-stu-id="f72ac-134">If your application sends by using the `/me` endpoint (or `/users/{user-id}` where the `user-id` corresponds to the signed in user), by default, the message will be saved in the sending user's Sent Items folder.</span></span>
- <span data-ttu-id="f72ac-135">Если ваше приложение выполняет отправку с использованием `/users/{user-id}`, где `user-id` соответствует пользователю, значащемуся в качестве отправителя, по умолчанию сообщение будет сохранено в папке "Отправленные" пользователя, значащегося как отправитель.</span><span class="sxs-lookup"><span data-stu-id="f72ac-135">If your application sends by using the `/users/{user-id}` where the `user-id` corresponds to the from user, by default, the message will be saved in the from user's Sent Items folder.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="f72ac-136">Чтобы отправить таким образом, фактический отправитель должен иметь разрешение для почтового ящика **Полный доступ**, помимо разрешения **Отправить от имени** или **Отправить как**.</span><span class="sxs-lookup"><span data-stu-id="f72ac-136">In order to send this way, the sending user must have the **Full Access** mailbox permission in addition to either the **Send on Behalf** or **Send As** permission.</span></span>

<span data-ttu-id="f72ac-137">Порядок по умолчанию может меняться в зависимости других сторонних факторов.</span><span class="sxs-lookup"><span data-stu-id="f72ac-137">The default behavior can be changed by other outside factors:</span></span>

- <span data-ttu-id="f72ac-138">Администраторы могут обновить почтовый ящик пользователя, значащегося в качестве отправителя, таким образом, чтобы [всегда сохранять копии сообщений, отправленных делегированным пользователем,](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) в его папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="f72ac-138">Administrators can update the from user's mailbox to [always save a copy of messages sent from a delegate](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) to their Sent Items.</span></span>
- <span data-ttu-id="f72ac-139">Задав свойство `saveToSentItems` как `false` в запросе [отправить почту](/graph/api/user-sendmail?view=graph-rest-1.0), вы можете отменить сохранение элемента в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="f72ac-139">By setting the `saveToSentItems` property to `false` in a [send mail](/graph/api/user-sendmail?view=graph-rest-1.0) request, you can prevent the item from being saved to the Sent Items folder.</span></span> <span data-ttu-id="f72ac-140">Тем не менее, если администратор настроил параметр "всегда сохранять копию", сообщения будут по-прежнему сохраняться в папке "Отправленные" пользователя, значащегося как отправитель.</span><span class="sxs-lookup"><span data-stu-id="f72ac-140">However, if an administrator has configured the "always save a copy" setting, the message will still be saved to the from user's Sent Items.</span></span>

## <a name="examples"></a><span data-ttu-id="f72ac-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="f72ac-141">Examples</span></span>

### <a name="example-1-successful-send-through-me-endpoint"></a><span data-ttu-id="f72ac-142">Пример 1. Успешная отправка через конечную точку /me endpoint</span><span class="sxs-lookup"><span data-stu-id="f72ac-142">Example 1: Successful send through /me endpoint</span></span>

<span data-ttu-id="f72ac-143">В этом примере Александру Воронову предоставлено разрешение **Отправить от имени** на почтовый ящик Алексея Виноградова.</span><span class="sxs-lookup"><span data-stu-id="f72ac-143">In this example, Adele Vance has been granted **Send on Behalf** permission to Allan Deyoung's mailbox.</span></span>

#### <a name="request"></a><span data-ttu-id="f72ac-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f72ac-144">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Expense reports",
    "body": {
      "contentType": "text",
      "content": "Have you submitted your expense reports yet?"
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "AllanD@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="f72ac-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="f72ac-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-unsuccessful-attempt-to-send-without-permissions"></a><span data-ttu-id="f72ac-146">Пример 2. Неудачная попытка отправки без разрешений</span><span class="sxs-lookup"><span data-stu-id="f72ac-146">Example 2: Unsuccessful attempt to send without permissions</span></span>

<span data-ttu-id="f72ac-147">В этом примере Александр Воронов пытается отправить сообщение электронной почты от Полины Кольцовой, однако ему не предоставлено разрешение **Отправить от имени** или **Отправить как**.</span><span class="sxs-lookup"><span data-stu-id="f72ac-147">In this example, Adele Vance attempts to send an email from Patti Fernandez, but has not been granted either the **Send on Behalf** or **Send As** permission.</span></span> <span data-ttu-id="f72ac-148">Ответ содержит ошибку `ErrorSendAsDenied`.</span><span class="sxs-lookup"><span data-stu-id="f72ac-148">The response contains a `ErrorSendAsDenied` error.</span></span>

<!-- markdownlint-disable MD024 -->

#### <a name="request"></a><span data-ttu-id="f72ac-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f72ac-149">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Support ticket",
    "body": {
      "contentType": "text",
      "content": "I noticed you opened a support ticket yesterday..."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "PattiF@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="f72ac-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="f72ac-150">Response</span></span>

```http
HTTP/1.1 403 Forbidden
Content-Type: application/json

{
  "error": {
    "code": "ErrorSendAsDenied",
    "message": "The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account. Cannot submit message.",
    "innerError": {
      "request-id": "24e7991e-01ae-4cc2-8e06-532a96fd8948",
      "date": "2019-01-16T18:53:25"
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="f72ac-151">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f72ac-151">Next steps</span></span>

<span data-ttu-id="f72ac-152">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="f72ac-152">Find out more about:</span></span>

- [<span data-ttu-id="f72ac-153">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="f72ac-153">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="f72ac-154">[Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [вариантов использования](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) API почты в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="f72ac-154">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and mail API [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox](always save a copy of messages sent from a delegate)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      InvalidUrlFormat '[/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide](Office 365 admin center)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/Exchange/recipients/mailbox-permissions](mailbox permissions)'. "
  ]
}
-->
