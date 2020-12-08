---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f675f8648b15f36517c1880f7bdb0c3178ef6b67
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597422"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="7c91e-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="7c91e-104">subscription resource type</span></span>

<span data-ttu-id="7c91e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c91e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c91e-106">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7c91e-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="7c91e-107">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7c91e-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="7c91e-108">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="7c91e-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="7c91e-109">[callRecord][], создаваемый после звонка или собрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c91e-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="7c91e-110">Объект [chatMessage][], отправленный в командах или каналах в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c91e-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="7c91e-111">[Беседа][] в группе Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="7c91e-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="7c91e-112">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c91e-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="7c91e-113">[Список][] на [сайте][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c91e-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="7c91e-114">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="7c91e-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="7c91e-115">[Присутствие][] пользователя в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c91e-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="7c91e-116">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7c91e-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="7c91e-117">[Принттаскдефинитион][] в службе печати</span><span class="sxs-lookup"><span data-stu-id="7c91e-117">A [printTaskDefinition][] in Print Service</span></span>
- <span data-ttu-id="7c91e-118">[Тодотаск] пользователя в корпорации Майкрософт</span><span class="sxs-lookup"><span data-stu-id="7c91e-118">A [todoTask] of a user in Microsoft To Do</span></span>

<span data-ttu-id="7c91e-119">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="7c91e-119">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="7c91e-120">Методы</span><span class="sxs-lookup"><span data-stu-id="7c91e-120">Methods</span></span>

| <span data-ttu-id="7c91e-121">Метод</span><span class="sxs-lookup"><span data-stu-id="7c91e-121">Method</span></span> | <span data-ttu-id="7c91e-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c91e-122">Return Type</span></span> | <span data-ttu-id="7c91e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7c91e-123">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="7c91e-124">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="7c91e-124">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="7c91e-125">subscription</span><span class="sxs-lookup"><span data-stu-id="7c91e-125">subscription</span></span>](subscription.md) | <span data-ttu-id="7c91e-126">Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7c91e-126">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="7c91e-127">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="7c91e-127">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="7c91e-128">subscription</span><span class="sxs-lookup"><span data-stu-id="7c91e-128">subscription</span></span>](subscription.md) | <span data-ttu-id="7c91e-129">Продлить подписку, обновив срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="7c91e-129">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="7c91e-130">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="7c91e-130">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="7c91e-131">subscription</span><span class="sxs-lookup"><span data-stu-id="7c91e-131">subscription</span></span>](subscription.md) | <span data-ttu-id="7c91e-132">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="7c91e-132">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="7c91e-133">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="7c91e-133">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="7c91e-134">subscription</span><span class="sxs-lookup"><span data-stu-id="7c91e-134">subscription</span></span>](subscription.md) | <span data-ttu-id="7c91e-135">Чтение свойств и связей объекта Subscription.</span><span class="sxs-lookup"><span data-stu-id="7c91e-135">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="7c91e-136">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="7c91e-136">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="7c91e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="7c91e-137">None</span></span> | <span data-ttu-id="7c91e-138">Удаление объекта подписки.</span><span class="sxs-lookup"><span data-stu-id="7c91e-138">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c91e-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c91e-139">Properties</span></span>

| <span data-ttu-id="7c91e-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c91e-140">Property</span></span> | <span data-ttu-id="7c91e-141">Тип</span><span class="sxs-lookup"><span data-stu-id="7c91e-141">Type</span></span> | <span data-ttu-id="7c91e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="7c91e-142">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7c91e-143">changeType</span><span class="sxs-lookup"><span data-stu-id="7c91e-143">changeType</span></span> | <span data-ttu-id="7c91e-144">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-144">string</span></span> | <span data-ttu-id="7c91e-145">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="7c91e-145">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="7c91e-146">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="7c91e-146">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="7c91e-147">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="7c91e-147">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="7c91e-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-148">Required.</span></span> <br><br><span data-ttu-id="7c91e-149">Примечание. Уведомления об изменении корневых элементов диска и списков поддерживают только changeType `updated`.</span><span class="sxs-lookup"><span data-stu-id="7c91e-149">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="7c91e-150">Уведомления об изменении пользователей и групп поддерживают changeType `updated` и `deleted`.</span><span class="sxs-lookup"><span data-stu-id="7c91e-150">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="7c91e-151">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="7c91e-151">notificationUrl</span></span> | <span data-ttu-id="7c91e-152">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-152">string</span></span> | <span data-ttu-id="7c91e-153">URL-адрес конечной точки, которая получает уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="7c91e-153">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="7c91e-154">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="7c91e-154">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="7c91e-155">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-155">Required.</span></span> |
| <span data-ttu-id="7c91e-156">лифецикленотификатионурл</span><span class="sxs-lookup"><span data-stu-id="7c91e-156">lifecycleNotificationUrl</span></span> | <span data-ttu-id="7c91e-157">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-157">string</span></span> | <span data-ttu-id="7c91e-158">URL-адрес конечной точки, которая получает уведомления жизненного цикла, включая `subscriptionRemoved` и `missed` уведомления.</span><span class="sxs-lookup"><span data-stu-id="7c91e-158">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="7c91e-159">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="7c91e-159">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="7c91e-160">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c91e-160">Optional.</span></span> <br><br><span data-ttu-id="7c91e-161">[Узнайте больше](/graph/webhooks-lifecycle) о том, как ресурсы Outlook используют Уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="7c91e-161">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="7c91e-162">resource</span><span class="sxs-lookup"><span data-stu-id="7c91e-162">resource</span></span> | <span data-ttu-id="7c91e-163">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-163">string</span></span> | <span data-ttu-id="7c91e-164">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="7c91e-164">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7c91e-165">Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="7c91e-165">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="7c91e-166">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7c91e-166">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="7c91e-167">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-167">Required.</span></span> |
| <span data-ttu-id="7c91e-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7c91e-168">expirationDateTime</span></span> | <span data-ttu-id="7c91e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c91e-169">DateTimeOffset</span></span> | <span data-ttu-id="7c91e-170">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="7c91e-170">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="7c91e-171">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="7c91e-171">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="7c91e-172">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="7c91e-172">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="7c91e-173">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-173">Required.</span></span> |
| <span data-ttu-id="7c91e-174">clientState</span><span class="sxs-lookup"><span data-stu-id="7c91e-174">clientState</span></span> | <span data-ttu-id="7c91e-175">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-175">string</span></span> | <span data-ttu-id="7c91e-176">Задает значение свойства **clientState** , которое отправляется службой в каждом уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="7c91e-176">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="7c91e-177">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="7c91e-177">The maximum length is 255 characters.</span></span> <span data-ttu-id="7c91e-178">Клиент может проверить, что уведомление об изменении поступило из службы, сравнив значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="7c91e-178">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="7c91e-179">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c91e-179">Optional.</span></span> |
| <span data-ttu-id="7c91e-180">id</span><span class="sxs-lookup"><span data-stu-id="7c91e-180">id</span></span> | <span data-ttu-id="7c91e-181">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-181">string</span></span> | <span data-ttu-id="7c91e-p110">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c91e-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="7c91e-184">applicationId</span><span class="sxs-lookup"><span data-stu-id="7c91e-184">applicationId</span></span> | <span data-ttu-id="7c91e-185">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-185">string</span></span> | <span data-ttu-id="7c91e-186">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="7c91e-186">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="7c91e-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c91e-187">Read-only.</span></span> |
| <span data-ttu-id="7c91e-188">creatorId</span><span class="sxs-lookup"><span data-stu-id="7c91e-188">creatorId</span></span> | <span data-ttu-id="7c91e-189">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-189">string</span></span> | <span data-ttu-id="7c91e-190">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="7c91e-190">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="7c91e-191">Если приложение использовало делегированные разрешения для создания подписки, это поле содержит идентификатор пользователя, выполнившего вход в систему, вызываемую приложением от имени.</span><span class="sxs-lookup"><span data-stu-id="7c91e-191">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="7c91e-192">Если приложение использовало разрешения приложения, это поле содержит идентификатор участника службы, соответствующего приложению.</span><span class="sxs-lookup"><span data-stu-id="7c91e-192">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="7c91e-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c91e-193">Read-only.</span></span> |
| <span data-ttu-id="7c91e-194">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="7c91e-194">includeResourceData</span></span> | <span data-ttu-id="7c91e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c91e-195">Boolean</span></span> | <span data-ttu-id="7c91e-196">Если присвоено значение `true`, уведомления об изменениях [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата).</span><span class="sxs-lookup"><span data-stu-id="7c91e-196">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="7c91e-197">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-197">Optional.</span></span> | 
| <span data-ttu-id="7c91e-198">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="7c91e-198">encryptionCertificate</span></span> | <span data-ttu-id="7c91e-199">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-199">string</span></span> | <span data-ttu-id="7c91e-200">Представление в кодировке Base64 сертификата с открытым ключом, используемое для шифрования данных ресурса в уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="7c91e-200">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="7c91e-201">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-201">Optional.</span></span> <span data-ttu-id="7c91e-202">Обязательно, если **includeResourceData** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="7c91e-202">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="7c91e-203">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="7c91e-203">encryptionCertificateId</span></span> | <span data-ttu-id="7c91e-204">string</span><span class="sxs-lookup"><span data-stu-id="7c91e-204">string</span></span> | <span data-ttu-id="7c91e-205">Предоставляемый приложением настраиваемый идентификатор, помогающий определить сертификат, необходимый для расшифровки данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="7c91e-205">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="7c91e-206">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7c91e-206">Optional.</span></span> <span data-ttu-id="7c91e-207">Обязательно, если **includeResourceData** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="7c91e-207">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="7c91e-208">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="7c91e-208">latestSupportedTlsVersion</span></span> | <span data-ttu-id="7c91e-209">Строка</span><span class="sxs-lookup"><span data-stu-id="7c91e-209">String</span></span> | <span data-ttu-id="7c91e-210">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7c91e-210">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="7c91e-211">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="7c91e-211">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="7c91e-212">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="7c91e-212">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="7c91e-213">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="7c91e-213">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="7c91e-214">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="7c91e-214">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="7c91e-215">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="7c91e-215">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="7c91e-216">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="7c91e-216">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="7c91e-217">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7c91e-217">Resource</span></span>            | <span data-ttu-id="7c91e-218">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="7c91e-218">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="7c91e-219">**Оповещение** безопасности</span><span class="sxs-lookup"><span data-stu-id="7c91e-219">Security **alert**</span></span>     | <span data-ttu-id="7c91e-220">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-220">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="7c91e-221">**callRecord** в Teams</span><span class="sxs-lookup"><span data-stu-id="7c91e-221">Teams **callRecord**</span></span>    | <span data-ttu-id="7c91e-222">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-222">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="7c91e-223">**chatMessage** в Teams</span><span class="sxs-lookup"><span data-stu-id="7c91e-223">Teams **chatMessage**</span></span>    | <span data-ttu-id="7c91e-224">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="7c91e-224">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="7c91e-225">Групповая **беседа**</span><span class="sxs-lookup"><span data-stu-id="7c91e-225">Group **conversation**</span></span> | <span data-ttu-id="7c91e-226">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-227">**driveItem** OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c91e-227">OneDrive **driveItem**</span></span>    | <span data-ttu-id="7c91e-228">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-229">**Список** SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c91e-229">SharePoint **list**</span></span>    | <span data-ttu-id="7c91e-230">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-230">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-231">**Сообщение**, **событие**, **контакт** Outlook</span><span class="sxs-lookup"><span data-stu-id="7c91e-231">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="7c91e-232">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-232">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-233">**Пользователь**, **группа**, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="7c91e-233">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="7c91e-234">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-234">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-235">**presence**</span><span class="sxs-lookup"><span data-stu-id="7c91e-235">**presence**</span></span>        | <span data-ttu-id="7c91e-236">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="7c91e-236">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="7c91e-237">Печать **принттаскдефинитион**</span><span class="sxs-lookup"><span data-stu-id="7c91e-237">Print **printTaskDefinition**</span></span> | <span data-ttu-id="7c91e-238">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-238">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="7c91e-239">**тодотаск**</span><span class="sxs-lookup"><span data-stu-id="7c91e-239">**todoTask**</span></span>              | <span data-ttu-id="7c91e-240">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="7c91e-240">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="7c91e-241">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="7c91e-241">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="7c91e-242">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="7c91e-242">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="7c91e-243">Отношения</span><span class="sxs-lookup"><span data-stu-id="7c91e-243">Relationships</span></span>

<span data-ttu-id="7c91e-244">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7c91e-244">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c91e-245">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c91e-245">JSON representation</span></span>

<span data-ttu-id="7c91e-246">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c91e-246">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string"
}
```

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md
[callRecord]: ./callrecords-callrecord.md
[presence]: ./presence.md
[printTaskDefinition]: ./printtaskdefinition.md
[тодотаск]: ./todotask.md
[todoTask]: ./todotask.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


