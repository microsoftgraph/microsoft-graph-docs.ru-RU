---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a82995a88b3dd5829b0f1f7c9b2cb5bcb5dfa18
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314659"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="2aeca-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="2aeca-104">subscription resource type</span></span>

<span data-ttu-id="2aeca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aeca-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2aeca-106">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2aeca-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="2aeca-107">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2aeca-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="2aeca-108">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="2aeca-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="2aeca-109">[callRecord][], создаваемый после звонка или собрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2aeca-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="2aeca-110">Объект [chatMessage][], отправленный в командах или каналах в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2aeca-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="2aeca-111">[Беседа][] в группе Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="2aeca-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="2aeca-112">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="2aeca-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="2aeca-113">[Список][] на [сайте][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="2aeca-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="2aeca-114">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="2aeca-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="2aeca-115">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2aeca-115">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="2aeca-116">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="2aeca-116">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="2aeca-117">Методы</span><span class="sxs-lookup"><span data-stu-id="2aeca-117">Methods</span></span>

| <span data-ttu-id="2aeca-118">Метод</span><span class="sxs-lookup"><span data-stu-id="2aeca-118">Method</span></span> | <span data-ttu-id="2aeca-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2aeca-119">Return Type</span></span> | <span data-ttu-id="2aeca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2aeca-120">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="2aeca-121">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2aeca-121">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="2aeca-122">subscription</span><span class="sxs-lookup"><span data-stu-id="2aeca-122">subscription</span></span>](subscription.md) | <span data-ttu-id="2aeca-123">Создает подписку для приложения прослушивателя, позволяющую получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2aeca-123">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="2aeca-124">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="2aeca-124">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="2aeca-125">subscription</span><span class="sxs-lookup"><span data-stu-id="2aeca-125">subscription</span></span>](subscription.md) | <span data-ttu-id="2aeca-126">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="2aeca-126">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="2aeca-127">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="2aeca-127">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="2aeca-128">subscription</span><span class="sxs-lookup"><span data-stu-id="2aeca-128">subscription</span></span>](subscription.md) | <span data-ttu-id="2aeca-129">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="2aeca-129">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="2aeca-130">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="2aeca-130">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="2aeca-131">subscription</span><span class="sxs-lookup"><span data-stu-id="2aeca-131">subscription</span></span>](subscription.md) | <span data-ttu-id="2aeca-132">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="2aeca-132">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="2aeca-133">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="2aeca-133">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="2aeca-134">Нет</span><span class="sxs-lookup"><span data-stu-id="2aeca-134">None</span></span> | <span data-ttu-id="2aeca-135">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="2aeca-135">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2aeca-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aeca-136">Properties</span></span>

| <span data-ttu-id="2aeca-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aeca-137">Property</span></span> | <span data-ttu-id="2aeca-138">Тип</span><span class="sxs-lookup"><span data-stu-id="2aeca-138">Type</span></span> | <span data-ttu-id="2aeca-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2aeca-139">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2aeca-140">changeType</span><span class="sxs-lookup"><span data-stu-id="2aeca-140">changeType</span></span> | <span data-ttu-id="2aeca-141">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-141">string</span></span> | <span data-ttu-id="2aeca-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2aeca-142">Required.</span></span> <span data-ttu-id="2aeca-143">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="2aeca-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="2aeca-144">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="2aeca-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="2aeca-145">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="2aeca-145">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="2aeca-146">Примечание. Уведомления об изменении корневых элементов диска и списков поддерживают только changeType `updated`.</span><span class="sxs-lookup"><span data-stu-id="2aeca-146">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="2aeca-147">Уведомления об изменении пользователей и групп поддерживают changeType `updated` и `deleted`.</span><span class="sxs-lookup"><span data-stu-id="2aeca-147">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="2aeca-148">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="2aeca-148">notificationUrl</span></span> | <span data-ttu-id="2aeca-149">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-149">string</span></span> | <span data-ttu-id="2aeca-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2aeca-150">Required.</span></span> <span data-ttu-id="2aeca-151">URL-адрес конечной точки, которая будет получать уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2aeca-151">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="2aeca-152">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="2aeca-152">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="2aeca-153">resource</span><span class="sxs-lookup"><span data-stu-id="2aeca-153">resource</span></span> | <span data-ttu-id="2aeca-154">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-154">string</span></span> | <span data-ttu-id="2aeca-155">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2aeca-155">Required.</span></span> <span data-ttu-id="2aeca-156">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="2aeca-156">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="2aeca-157">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="2aeca-157">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="2aeca-158">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2aeca-158">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="2aeca-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2aeca-159">expirationDateTime</span></span> | [<span data-ttu-id="2aeca-160">dateTime</span><span class="sxs-lookup"><span data-stu-id="2aeca-160">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="2aeca-161">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2aeca-161">Required.</span></span> <span data-ttu-id="2aeca-162">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="2aeca-162">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="2aeca-163">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="2aeca-163">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="2aeca-164">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="2aeca-164">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="2aeca-165">clientState</span><span class="sxs-lookup"><span data-stu-id="2aeca-165">clientState</span></span> | <span data-ttu-id="2aeca-166">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-166">string</span></span> | <span data-ttu-id="2aeca-167">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2aeca-167">Optional.</span></span> <span data-ttu-id="2aeca-168">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="2aeca-168">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="2aeca-169">Максимальная длина — 128 символов.</span><span class="sxs-lookup"><span data-stu-id="2aeca-169">The maximum length is 128 characters.</span></span> <span data-ttu-id="2aeca-170">Клиент может проверить, пришло ли уведомление об изменении от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="2aeca-170">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="2aeca-171">id</span><span class="sxs-lookup"><span data-stu-id="2aeca-171">id</span></span> | <span data-ttu-id="2aeca-172">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-172">string</span></span> | <span data-ttu-id="2aeca-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2aeca-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="2aeca-175">applicationId</span><span class="sxs-lookup"><span data-stu-id="2aeca-175">applicationId</span></span> | <span data-ttu-id="2aeca-176">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-176">string</span></span> | <span data-ttu-id="2aeca-177">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="2aeca-177">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="2aeca-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2aeca-178">Read-only.</span></span> |
| <span data-ttu-id="2aeca-179">creatorId</span><span class="sxs-lookup"><span data-stu-id="2aeca-179">creatorId</span></span> | <span data-ttu-id="2aeca-180">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-180">string</span></span> | <span data-ttu-id="2aeca-181">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="2aeca-181">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="2aeca-182">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="2aeca-182">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="2aeca-183">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="2aeca-183">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="2aeca-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2aeca-184">Read-only.</span></span> |
| <span data-ttu-id="2aeca-185">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="2aeca-185">includeResourceData</span></span> | <span data-ttu-id="2aeca-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2aeca-186">Boolean</span></span> | <span data-ttu-id="2aeca-187">Если присвоено значение `true`, уведомления об изменениях [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата).</span><span class="sxs-lookup"><span data-stu-id="2aeca-187">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="2aeca-188">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2aeca-188">Optional.</span></span> | 
| <span data-ttu-id="2aeca-189">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="2aeca-189">encryptionCertificate</span></span> | <span data-ttu-id="2aeca-190">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-190">string</span></span> | <span data-ttu-id="2aeca-191">Представление в кодировке Base64 сертификата с открытым ключом, используемое для шифрования данных ресурса в уведомлениях об изменениях.</span><span class="sxs-lookup"><span data-stu-id="2aeca-191">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="2aeca-192">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2aeca-192">Optional.</span></span> <span data-ttu-id="2aeca-193">Обязательно, если **includeResourceData** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="2aeca-193">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="2aeca-194">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="2aeca-194">encryptionCertificateId</span></span> | <span data-ttu-id="2aeca-195">string</span><span class="sxs-lookup"><span data-stu-id="2aeca-195">string</span></span> | <span data-ttu-id="2aeca-196">Предоставляемый приложением настраиваемый идентификатор, помогающий определить сертификат, необходимый для расшифровки данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="2aeca-196">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="2aeca-197">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2aeca-197">Optional.</span></span> 
| <span data-ttu-id="2aeca-198">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="2aeca-198">latestSupportedTlsVersion</span></span> | <span data-ttu-id="2aeca-199">Строка</span><span class="sxs-lookup"><span data-stu-id="2aeca-199">String</span></span> | <span data-ttu-id="2aeca-200">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="2aeca-200">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="2aeca-201">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="2aeca-201">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="2aeca-202">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="2aeca-202">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="2aeca-203">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="2aeca-203">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="2aeca-204">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="2aeca-204">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="2aeca-205">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="2aeca-205">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="2aeca-206">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="2aeca-206">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="2aeca-207">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2aeca-207">Resource</span></span>            | <span data-ttu-id="2aeca-208">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="2aeca-208">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="2aeca-209">**Оповещение** безопасности</span><span class="sxs-lookup"><span data-stu-id="2aeca-209">Security **alert**</span></span>     | <span data-ttu-id="2aeca-210">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-210">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="2aeca-211">**callRecord** в Teams</span><span class="sxs-lookup"><span data-stu-id="2aeca-211">Teams **callRecord**</span></span>    | <span data-ttu-id="2aeca-212">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-212">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="2aeca-213">**chatMessage** в Teams</span><span class="sxs-lookup"><span data-stu-id="2aeca-213">Teams **chatMessage**</span></span>    | <span data-ttu-id="2aeca-214">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="2aeca-214">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="2aeca-215">Групповая **беседа**</span><span class="sxs-lookup"><span data-stu-id="2aeca-215">Group **conversation**</span></span> | <span data-ttu-id="2aeca-216">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-216">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2aeca-217">**driveItem** OneDrive</span><span class="sxs-lookup"><span data-stu-id="2aeca-217">OneDrive **driveItem**</span></span>    | <span data-ttu-id="2aeca-218">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-218">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2aeca-219">**Список** SharePoint</span><span class="sxs-lookup"><span data-stu-id="2aeca-219">SharePoint **list**</span></span>    | <span data-ttu-id="2aeca-220">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-220">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2aeca-221">**Сообщение**, **событие**, **контакт** Outlook</span><span class="sxs-lookup"><span data-stu-id="2aeca-221">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="2aeca-222">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-222">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="2aeca-223">**Пользователь**, **группа**, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="2aeca-223">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="2aeca-224">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="2aeca-224">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="2aeca-225">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="2aeca-225">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="2aeca-226">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2aeca-226">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="2aeca-227">Отношения</span><span class="sxs-lookup"><span data-stu-id="2aeca-227">Relationships</span></span>

<span data-ttu-id="2aeca-228">Нет</span><span class="sxs-lookup"><span data-stu-id="2aeca-228">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aeca-229">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aeca-229">JSON representation</span></span>

<span data-ttu-id="2aeca-230">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aeca-230">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

