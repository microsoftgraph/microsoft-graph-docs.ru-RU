---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2639e23181af020722311cb6db00c9464949725a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897654"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="0d05a-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="0d05a-104">subscription resource type</span></span>

<span data-ttu-id="0d05a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d05a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d05a-106">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d05a-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="0d05a-107">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0d05a-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="0d05a-108">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="0d05a-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="0d05a-109">[Каллрекорд][] , созданный после вызова или собрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0d05a-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="0d05a-110">[Беседа][] в группе Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0d05a-110">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="0d05a-111">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d05a-111">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="0d05a-112">[Список][] на [сайте][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="0d05a-112">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="0d05a-113">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="0d05a-113">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="0d05a-114">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0d05a-114">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="0d05a-115">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="0d05a-115">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="0d05a-116">Методы</span><span class="sxs-lookup"><span data-stu-id="0d05a-116">Methods</span></span>

| <span data-ttu-id="0d05a-117">Метод</span><span class="sxs-lookup"><span data-stu-id="0d05a-117">Method</span></span> | <span data-ttu-id="0d05a-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d05a-118">Return Type</span></span> | <span data-ttu-id="0d05a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0d05a-119">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="0d05a-120">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="0d05a-120">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="0d05a-121">subscription</span><span class="sxs-lookup"><span data-stu-id="0d05a-121">subscription</span></span>](subscription.md) | <span data-ttu-id="0d05a-122">Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d05a-122">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="0d05a-123">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="0d05a-123">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="0d05a-124">subscription</span><span class="sxs-lookup"><span data-stu-id="0d05a-124">subscription</span></span>](subscription.md) | <span data-ttu-id="0d05a-125">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="0d05a-125">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="0d05a-126">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="0d05a-126">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="0d05a-127">subscription</span><span class="sxs-lookup"><span data-stu-id="0d05a-127">subscription</span></span>](subscription.md) | <span data-ttu-id="0d05a-128">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="0d05a-128">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="0d05a-129">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="0d05a-129">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="0d05a-130">subscription</span><span class="sxs-lookup"><span data-stu-id="0d05a-130">subscription</span></span>](subscription.md) | <span data-ttu-id="0d05a-131">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="0d05a-131">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="0d05a-132">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="0d05a-132">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="0d05a-133">Нет</span><span class="sxs-lookup"><span data-stu-id="0d05a-133">None</span></span> | <span data-ttu-id="0d05a-134">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="0d05a-134">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d05a-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d05a-135">Properties</span></span>

| <span data-ttu-id="0d05a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d05a-136">Property</span></span> | <span data-ttu-id="0d05a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0d05a-137">Type</span></span> | <span data-ttu-id="0d05a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0d05a-138">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="0d05a-139">changeType</span><span class="sxs-lookup"><span data-stu-id="0d05a-139">changeType</span></span> | <span data-ttu-id="0d05a-140">строка</span><span class="sxs-lookup"><span data-stu-id="0d05a-140">string</span></span> | <span data-ttu-id="0d05a-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d05a-141">Required.</span></span> <span data-ttu-id="0d05a-142">Указывает тип изменения в подписанном ресурсе, который будет вызывать уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="0d05a-142">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="0d05a-143">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="0d05a-143">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="0d05a-144">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="0d05a-144">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="0d05a-145">Note: корневой элемент диска и уведомления об изменении списка поддерживают только `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="0d05a-145">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="0d05a-146">Поддержка и ChangeType уведомлений об изменениях для пользователей и групп `updated` `deleted` .</span><span class="sxs-lookup"><span data-stu-id="0d05a-146">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="0d05a-147">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="0d05a-147">notificationUrl</span></span> | <span data-ttu-id="0d05a-148">строка</span><span class="sxs-lookup"><span data-stu-id="0d05a-148">string</span></span> | <span data-ttu-id="0d05a-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d05a-149">Required.</span></span> <span data-ttu-id="0d05a-150">URL-адрес конечной точки, которая будет получать уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="0d05a-150">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="0d05a-151">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="0d05a-151">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="0d05a-152">resource</span><span class="sxs-lookup"><span data-stu-id="0d05a-152">resource</span></span> | <span data-ttu-id="0d05a-153">строка</span><span class="sxs-lookup"><span data-stu-id="0d05a-153">string</span></span> | <span data-ttu-id="0d05a-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d05a-154">Required.</span></span> <span data-ttu-id="0d05a-155">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="0d05a-155">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="0d05a-156">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="0d05a-156">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="0d05a-157">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0d05a-157">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="0d05a-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0d05a-158">expirationDateTime</span></span> | [<span data-ttu-id="0d05a-159">dateTime</span><span class="sxs-lookup"><span data-stu-id="0d05a-159">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="0d05a-160">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0d05a-160">Required.</span></span> <span data-ttu-id="0d05a-161">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="0d05a-161">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="0d05a-162">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="0d05a-162">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="0d05a-163">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="0d05a-163">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="0d05a-164">clientState</span><span class="sxs-lookup"><span data-stu-id="0d05a-164">clientState</span></span> | <span data-ttu-id="0d05a-165">строка</span><span class="sxs-lookup"><span data-stu-id="0d05a-165">string</span></span> | <span data-ttu-id="0d05a-166">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0d05a-166">Optional.</span></span> <span data-ttu-id="0d05a-167">Задает значение `clientState` свойства, отправленного службой в каждом уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="0d05a-167">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="0d05a-168">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="0d05a-168">The maximum length is 128 characters.</span></span> <span data-ttu-id="0d05a-169">Клиент может проверить, что уведомление об изменении поступило из службы, сравнив значение свойства, `clientState` отправленного с подпиской, со значением свойства, `clientState` полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="0d05a-169">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="0d05a-170">id</span><span class="sxs-lookup"><span data-stu-id="0d05a-170">id</span></span> | <span data-ttu-id="0d05a-171">string</span><span class="sxs-lookup"><span data-stu-id="0d05a-171">string</span></span> | <span data-ttu-id="0d05a-172">Unique identifier for the subscription.</span><span class="sxs-lookup"><span data-stu-id="0d05a-172">Unique identifier for the subscription.</span></span> <span data-ttu-id="0d05a-173">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0d05a-173">Read-only.</span></span> |
| <span data-ttu-id="0d05a-174">applicationId</span><span class="sxs-lookup"><span data-stu-id="0d05a-174">applicationId</span></span> | <span data-ttu-id="0d05a-175">string</span><span class="sxs-lookup"><span data-stu-id="0d05a-175">string</span></span> | <span data-ttu-id="0d05a-176">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="0d05a-176">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="0d05a-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d05a-177">Read-only.</span></span> |
| <span data-ttu-id="0d05a-178">creatorId</span><span class="sxs-lookup"><span data-stu-id="0d05a-178">creatorId</span></span> | <span data-ttu-id="0d05a-179">string</span><span class="sxs-lookup"><span data-stu-id="0d05a-179">string</span></span> | <span data-ttu-id="0d05a-180">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="0d05a-180">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="0d05a-181">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="0d05a-181">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="0d05a-182">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="0d05a-182">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="0d05a-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d05a-183">Read-only.</span></span> |
| <span data-ttu-id="0d05a-184">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="0d05a-184">latestSupportedTlsVersion</span></span> | <span data-ttu-id="0d05a-185">Строка</span><span class="sxs-lookup"><span data-stu-id="0d05a-185">String</span></span> | <span data-ttu-id="0d05a-186">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="0d05a-186">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="0d05a-187">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="0d05a-187">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="0d05a-188">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="0d05a-188">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="0d05a-189">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="0d05a-189">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="0d05a-190">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="0d05a-190">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="0d05a-191">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="0d05a-191">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="0d05a-192">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="0d05a-192">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="0d05a-193">Ресурс</span><span class="sxs-lookup"><span data-stu-id="0d05a-193">Resource</span></span>            | <span data-ttu-id="0d05a-194">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="0d05a-194">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="0d05a-195">Пользователь, группа, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="0d05a-195">User, group, other directory resources</span></span>   | <span data-ttu-id="0d05a-196">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-197">Почта</span><span class="sxs-lookup"><span data-stu-id="0d05a-197">Mail</span></span>                | <span data-ttu-id="0d05a-198">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-199">Календарь</span><span class="sxs-lookup"><span data-stu-id="0d05a-199">Calendar</span></span>            | <span data-ttu-id="0d05a-200">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-201">Контакты</span><span class="sxs-lookup"><span data-stu-id="0d05a-201">Contacts</span></span>            | <span data-ttu-id="0d05a-202">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-203">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="0d05a-203">Group conversations</span></span> | <span data-ttu-id="0d05a-204">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-204">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-205">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="0d05a-205">Drive root items</span></span>    | <span data-ttu-id="0d05a-206">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-206">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-207">Список SharePoint</span><span class="sxs-lookup"><span data-stu-id="0d05a-207">SharePoint list</span></span>     | <span data-ttu-id="0d05a-208">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-208">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0d05a-209">Каллрекорд Teams</span><span class="sxs-lookup"><span data-stu-id="0d05a-209">Teams callRecord</span></span>    | <span data-ttu-id="0d05a-210">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-210">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="0d05a-211">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="0d05a-211">Security alerts</span></span>     | <span data-ttu-id="0d05a-212">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="0d05a-212">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="0d05a-213">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="0d05a-213">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="0d05a-214">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="0d05a-214">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="0d05a-215">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d05a-215">Relationships</span></span>

<span data-ttu-id="0d05a-216">Нет</span><span class="sxs-lookup"><span data-stu-id="0d05a-216">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d05a-217">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d05a-217">JSON representation</span></span>

<span data-ttu-id="0d05a-218">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d05a-218">Here is a JSON representation of the resource.</span></span>

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
