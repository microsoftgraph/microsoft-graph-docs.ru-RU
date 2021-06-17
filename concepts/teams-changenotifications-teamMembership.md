---
title: Получение уведомлений о любых изменениях участников Teams с помощью Microsoft Graph
description: Получение уведомлений о любых изменениях (создание, обновление и удаление) участников Teams с помощью Microsoft Graph
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 8f9d0a654f3105c7d365bc92f774ab66be34f35d
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971466"
---
# <a name="get-change-notifications-for-changes-in-teams-membership-using-microsoft-graph"></a><span data-ttu-id="39a7d-103">Получение уведомлений об изменениях участников Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39a7d-103">Get change notifications for changes in Teams membership using Microsoft Graph</span></span>

<span data-ttu-id="39a7d-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) участников команд.</span><span class="sxs-lookup"><span data-stu-id="39a7d-104">Change notifications enable you to subscribe to changes (create, update, and delete) in teams membership.</span></span> <span data-ttu-id="39a7d-105">Вы можете получать уведомления при добавлении, удалении или изменении участника в команде.</span><span class="sxs-lookup"><span data-stu-id="39a7d-105">You can get notified whenever member is added, removed or updated in a team.</span></span> <span data-ttu-id="39a7d-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="39a7d-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a><span data-ttu-id="39a7d-107">Подписка на изменения участников определенной команды</span><span class="sxs-lookup"><span data-stu-id="39a7d-107">Subscribe to changes in membership of a particular team</span></span>

<span data-ttu-id="39a7d-108">Чтобы получать уведомления об изменениях участников определенной команды, подпишитесь на `/teams/{id}/members`.</span><span class="sxs-lookup"><span data-stu-id="39a7d-108">To get change notifications for membership changes in a particular team, subscribe to `/teams/{id}/members`.</span></span> <span data-ttu-id="39a7d-109">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="39a7d-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="39a7d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39a7d-110">Permissions</span></span>

|<span data-ttu-id="39a7d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39a7d-111">Permission type</span></span>      | <span data-ttu-id="39a7d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39a7d-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="39a7d-113">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="39a7d-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="39a7d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39a7d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="39a7d-115">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="39a7d-115">TeamMember.Read.All</span></span> | <span data-ttu-id="39a7d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a7d-116">Not supported.</span></span> |
|<span data-ttu-id="39a7d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39a7d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a7d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a7d-118">Not supported.</span></span>    | <span data-ttu-id="39a7d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a7d-119">Not supported.</span></span> |
|<span data-ttu-id="39a7d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="39a7d-120">Application</span></span> | <span data-ttu-id="39a7d-121">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="39a7d-121">TeamMember.Read.All</span></span>   | <span data-ttu-id="39a7d-122">бета</span><span class="sxs-lookup"><span data-stu-id="39a7d-122">beta</span></span> |

#### <a name="example"></a><span data-ttu-id="39a7d-123">Пример</span><span class="sxs-lookup"><span data-stu-id="39a7d-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="39a7d-124">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="39a7d-124">Notifications with resource data</span></span>

<span data-ttu-id="39a7d-125">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="39a7d-125">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="39a7d-126">Эти полезные данные относятся к изменению участников в команде.</span><span class="sxs-lookup"><span data-stu-id="39a7d-126">This payload is for a membership change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
        "resourceData": {
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
            "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="39a7d-127">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="39a7d-127">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="39a7d-128">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="39a7d-128">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="39a7d-129">Полезные данные соответствуют схеме [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="39a7d-129">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="39a7d-130">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="39a7d-130">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [
    "owner"
  ],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="39a7d-131">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="39a7d-131">Notifications without resource data</span></span>

<span data-ttu-id="39a7d-132">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="39a7d-132">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="39a7d-133">Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).</span><span class="sxs-lookup"><span data-stu-id="39a7d-133">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="39a7d-134">Для уведомлений без данных ресурса полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="39a7d-134">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="39a7d-135">Эти полезные данные относятся к изменению участников в команде.</span><span class="sxs-lookup"><span data-stu-id="39a7d-135">This payload is for a membership change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
  "resourceData": {
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk",
    "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
    "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
  }
}
```

<span data-ttu-id="39a7d-136">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="39a7d-136">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="39a7d-137">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="39a7d-137">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="39a7d-138">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="39a7d-138">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="39a7d-139">См. также</span><span class="sxs-lookup"><span data-stu-id="39a7d-139">See also</span></span>
- [<span data-ttu-id="39a7d-140">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39a7d-140">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="39a7d-141">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="39a7d-141">Microsoft Teams API overview</span></span>](teams-concept-overview.md)