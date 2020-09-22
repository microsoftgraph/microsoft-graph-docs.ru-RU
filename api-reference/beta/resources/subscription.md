---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: aaa7fe900852f00851cafea2c18e71ec7fec7c8c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193332"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="b6996-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="b6996-104">subscription resource type</span></span>

<span data-ttu-id="b6996-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6996-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6996-106">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6996-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="b6996-107">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b6996-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="b6996-108">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="b6996-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="b6996-109">[callRecord][], создаваемый после звонка или собрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b6996-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="b6996-110">[ChatMessage][] , отправленный через Teams или каналы в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b6996-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="b6996-111">[Беседа][] в группе Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="b6996-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="b6996-112">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6996-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="b6996-113">[Список][] на [сайте][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="b6996-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="b6996-114">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="b6996-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="b6996-115">[Присутствие][] пользователя в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b6996-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="b6996-116">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b6996-116">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="b6996-117">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="b6996-117">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="b6996-118">Методы</span><span class="sxs-lookup"><span data-stu-id="b6996-118">Methods</span></span>

| <span data-ttu-id="b6996-119">Метод</span><span class="sxs-lookup"><span data-stu-id="b6996-119">Method</span></span> | <span data-ttu-id="b6996-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6996-120">Return Type</span></span> | <span data-ttu-id="b6996-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b6996-121">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="b6996-122">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="b6996-122">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b6996-123">subscription</span><span class="sxs-lookup"><span data-stu-id="b6996-123">subscription</span></span>](subscription.md) | <span data-ttu-id="b6996-124">Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6996-124">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="b6996-125">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="b6996-125">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="b6996-126">subscription</span><span class="sxs-lookup"><span data-stu-id="b6996-126">subscription</span></span>](subscription.md) | <span data-ttu-id="b6996-127">Продлить подписку, обновив срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="b6996-127">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="b6996-128">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="b6996-128">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="b6996-129">subscription</span><span class="sxs-lookup"><span data-stu-id="b6996-129">subscription</span></span>](subscription.md) | <span data-ttu-id="b6996-130">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="b6996-130">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="b6996-131">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="b6996-131">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="b6996-132">subscription</span><span class="sxs-lookup"><span data-stu-id="b6996-132">subscription</span></span>](subscription.md) | <span data-ttu-id="b6996-133">Чтение свойств и связей объекта Subscription.</span><span class="sxs-lookup"><span data-stu-id="b6996-133">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="b6996-134">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="b6996-134">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="b6996-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b6996-135">None</span></span> | <span data-ttu-id="b6996-136">Удаление объекта подписки.</span><span class="sxs-lookup"><span data-stu-id="b6996-136">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6996-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6996-137">Properties</span></span>

| <span data-ttu-id="b6996-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6996-138">Property</span></span> | <span data-ttu-id="b6996-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b6996-139">Type</span></span> | <span data-ttu-id="b6996-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b6996-140">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b6996-141">changeType</span><span class="sxs-lookup"><span data-stu-id="b6996-141">changeType</span></span> | <span data-ttu-id="b6996-142">string</span><span class="sxs-lookup"><span data-stu-id="b6996-142">string</span></span> | <span data-ttu-id="b6996-143">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="b6996-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="b6996-144">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b6996-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="b6996-145">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="b6996-145">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="b6996-146">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-146">Required.</span></span> <br><br><span data-ttu-id="b6996-147">Примечание. Уведомления об изменении корневых элементов диска и списков поддерживают только changeType `updated`.</span><span class="sxs-lookup"><span data-stu-id="b6996-147">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="b6996-148">Уведомления об изменении пользователей и групп поддерживают changeType `updated` и `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b6996-148">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="b6996-149">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="b6996-149">notificationUrl</span></span> | <span data-ttu-id="b6996-150">string</span><span class="sxs-lookup"><span data-stu-id="b6996-150">string</span></span> | <span data-ttu-id="b6996-151">URL-адрес конечной точки, которая получает уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="b6996-151">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="b6996-152">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="b6996-152">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="b6996-153">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-153">Required.</span></span> |
| <span data-ttu-id="b6996-154">лифецикленотификатионурл</span><span class="sxs-lookup"><span data-stu-id="b6996-154">lifecycleNotificationUrl</span></span> | <span data-ttu-id="b6996-155">string</span><span class="sxs-lookup"><span data-stu-id="b6996-155">string</span></span> | <span data-ttu-id="b6996-156">URL-адрес конечной точки, которая получает уведомления жизненного цикла, включая `subscriptionRemoved` и `missed` уведомления.</span><span class="sxs-lookup"><span data-stu-id="b6996-156">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="b6996-157">Если этот параметр не указан, уведомления будут доставляться в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="b6996-157">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="b6996-158">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="b6996-158">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="b6996-159">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-159">Optional.</span></span> <br><br><span data-ttu-id="b6996-160">[Узнайте больше](/graph/webhooks-outlook-authz) о том, как ресурсы Outlook используют Уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="b6996-160">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="b6996-161">resource</span><span class="sxs-lookup"><span data-stu-id="b6996-161">resource</span></span> | <span data-ttu-id="b6996-162">string</span><span class="sxs-lookup"><span data-stu-id="b6996-162">string</span></span> | <span data-ttu-id="b6996-163">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="b6996-163">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="b6996-164">Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="b6996-164">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="b6996-165">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b6996-165">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="b6996-166">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-166">Required.</span></span> |
| <span data-ttu-id="b6996-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b6996-167">expirationDateTime</span></span> | <span data-ttu-id="b6996-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6996-168">DateTimeOffset</span></span> | <span data-ttu-id="b6996-169">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="b6996-169">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="b6996-170">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="b6996-170">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="b6996-171">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="b6996-171">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="b6996-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-172">Required.</span></span> |
| <span data-ttu-id="b6996-173">clientState</span><span class="sxs-lookup"><span data-stu-id="b6996-173">clientState</span></span> | <span data-ttu-id="b6996-174">string</span><span class="sxs-lookup"><span data-stu-id="b6996-174">string</span></span> | <span data-ttu-id="b6996-175">Задает значение свойства **clientState** , которое отправляется службой в каждом уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="b6996-175">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="b6996-176">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="b6996-176">The maximum length is 255 characters.</span></span> <span data-ttu-id="b6996-177">Клиент может проверить, что уведомление об изменении поступило из службы, сравнив значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="b6996-177">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="b6996-178">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-178">Optional.</span></span> |
| <span data-ttu-id="b6996-179">id</span><span class="sxs-lookup"><span data-stu-id="b6996-179">id</span></span> | <span data-ttu-id="b6996-180">string</span><span class="sxs-lookup"><span data-stu-id="b6996-180">string</span></span> | <span data-ttu-id="b6996-p110">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6996-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="b6996-183">applicationId</span><span class="sxs-lookup"><span data-stu-id="b6996-183">applicationId</span></span> | <span data-ttu-id="b6996-184">string</span><span class="sxs-lookup"><span data-stu-id="b6996-184">string</span></span> | <span data-ttu-id="b6996-185">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="b6996-185">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="b6996-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6996-186">Read-only.</span></span> |
| <span data-ttu-id="b6996-187">creatorId</span><span class="sxs-lookup"><span data-stu-id="b6996-187">creatorId</span></span> | <span data-ttu-id="b6996-188">string</span><span class="sxs-lookup"><span data-stu-id="b6996-188">string</span></span> | <span data-ttu-id="b6996-189">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="b6996-189">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="b6996-190">Если приложение использовало делегированные разрешения для создания подписки, это поле содержит идентификатор пользователя, выполнившего вход в систему, вызываемую приложением от имени.</span><span class="sxs-lookup"><span data-stu-id="b6996-190">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="b6996-191">Если приложение использовало разрешения приложения, это поле содержит идентификатор участника службы, соответствующего приложению.</span><span class="sxs-lookup"><span data-stu-id="b6996-191">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="b6996-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6996-192">Read-only.</span></span> |
| <span data-ttu-id="b6996-193">инклудересаурцедата</span><span class="sxs-lookup"><span data-stu-id="b6996-193">includeResourceData</span></span> | <span data-ttu-id="b6996-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="b6996-194">Boolean</span></span> | <span data-ttu-id="b6996-195">Если задано значение `true` , уведомления об изменении [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата).</span><span class="sxs-lookup"><span data-stu-id="b6996-195">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="b6996-196">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-196">Optional.</span></span> | 
| <span data-ttu-id="b6996-197">енкриптионцертификате</span><span class="sxs-lookup"><span data-stu-id="b6996-197">encryptionCertificate</span></span> | <span data-ttu-id="b6996-198">string</span><span class="sxs-lookup"><span data-stu-id="b6996-198">string</span></span> | <span data-ttu-id="b6996-199">Представление сертификата с кодировкой base64 с открытым ключом, используемым для шифрования данных ресурсов в уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="b6996-199">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="b6996-200">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-200">Optional.</span></span> <span data-ttu-id="b6996-201">Является обязательным, если **инклудересаурцедата** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="b6996-201">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="b6996-202">енкриптионцертификатеид</span><span class="sxs-lookup"><span data-stu-id="b6996-202">encryptionCertificateId</span></span> | <span data-ttu-id="b6996-203">string</span><span class="sxs-lookup"><span data-stu-id="b6996-203">string</span></span> | <span data-ttu-id="b6996-204">Настраиваемый идентификатор, предоставляемый приложением, для определения сертификата, необходимого для расшифровки данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="b6996-204">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="b6996-205">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b6996-205">Optional.</span></span> <span data-ttu-id="b6996-206">Является обязательным, если **инклудересаурцедата** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="b6996-206">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="b6996-207">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="b6996-207">latestSupportedTlsVersion</span></span> | <span data-ttu-id="b6996-208">Строка</span><span class="sxs-lookup"><span data-stu-id="b6996-208">String</span></span> | <span data-ttu-id="b6996-209">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="b6996-209">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="b6996-210">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="b6996-210">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="b6996-211">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="b6996-211">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="b6996-212">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="b6996-212">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="b6996-213">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="b6996-213">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="b6996-214">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="b6996-214">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="b6996-215">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="b6996-215">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="b6996-216">Ресурс</span><span class="sxs-lookup"><span data-stu-id="b6996-216">Resource</span></span>            | <span data-ttu-id="b6996-217">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="b6996-217">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="b6996-218">**Оповещение** безопасности</span><span class="sxs-lookup"><span data-stu-id="b6996-218">Security **alert**</span></span>     | <span data-ttu-id="b6996-219">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-219">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="b6996-220">**callRecord** в Teams</span><span class="sxs-lookup"><span data-stu-id="b6996-220">Teams **callRecord**</span></span>    | <span data-ttu-id="b6996-221">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-221">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="b6996-222">**chatMessage** Teams</span><span class="sxs-lookup"><span data-stu-id="b6996-222">Teams **chatMessage**</span></span>    | <span data-ttu-id="b6996-223">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="b6996-223">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="b6996-224">Групповая **беседа**</span><span class="sxs-lookup"><span data-stu-id="b6996-224">Group **conversation**</span></span> | <span data-ttu-id="b6996-225">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-225">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b6996-226">OneDrive для **driveItem**</span><span class="sxs-lookup"><span data-stu-id="b6996-226">OneDrive **driveItem**</span></span>    | <span data-ttu-id="b6996-227">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b6996-228">**Список** SharePoint</span><span class="sxs-lookup"><span data-stu-id="b6996-228">SharePoint **list**</span></span>    | <span data-ttu-id="b6996-229">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b6996-230">**Сообщение**Outlook, **событие**, **контакт**</span><span class="sxs-lookup"><span data-stu-id="b6996-230">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="b6996-231">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-231">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b6996-232">**Пользователи**, **группы**и другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="b6996-232">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="b6996-233">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="b6996-233">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b6996-234">**presence**</span><span class="sxs-lookup"><span data-stu-id="b6996-234">**presence**</span></span>        | <span data-ttu-id="b6996-235">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="b6996-235">60 minutes (1 hour)</span></span> |


> <span data-ttu-id="b6996-236">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="b6996-236">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="b6996-237">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="b6996-237">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="b6996-238">Отношения</span><span class="sxs-lookup"><span data-stu-id="b6996-238">Relationships</span></span>

<span data-ttu-id="b6996-239">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b6996-239">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6996-240">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b6996-240">JSON representation</span></span>

<span data-ttu-id="b6996-241">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6996-241">Here is a JSON representation of the resource.</span></span>

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


