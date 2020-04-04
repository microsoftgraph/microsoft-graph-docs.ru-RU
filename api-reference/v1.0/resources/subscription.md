---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8ede2274abebbba1148762f5d3606cd61a4578a4
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108433"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="43a2e-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="43a2e-104">subscription resource type</span></span>

<span data-ttu-id="43a2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43a2e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43a2e-106">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="43a2e-106">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="43a2e-107">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="43a2e-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="43a2e-108">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="43a2e-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="43a2e-109">[Беседа][] в группе Office 365</span><span class="sxs-lookup"><span data-stu-id="43a2e-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="43a2e-110">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="43a2e-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="43a2e-111">[Список][] на [сайте][] SharePoint</span><span class="sxs-lookup"><span data-stu-id="43a2e-111">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="43a2e-112">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="43a2e-112">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="43a2e-113">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="43a2e-113">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="43a2e-114">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="43a2e-114">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="43a2e-115">Методы</span><span class="sxs-lookup"><span data-stu-id="43a2e-115">Methods</span></span>

| <span data-ttu-id="43a2e-116">Метод</span><span class="sxs-lookup"><span data-stu-id="43a2e-116">Method</span></span> | <span data-ttu-id="43a2e-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="43a2e-117">Return Type</span></span> | <span data-ttu-id="43a2e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="43a2e-118">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="43a2e-119">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="43a2e-119">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="43a2e-120">subscription</span><span class="sxs-lookup"><span data-stu-id="43a2e-120">subscription</span></span>](subscription.md) | <span data-ttu-id="43a2e-121">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="43a2e-121">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="43a2e-122">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="43a2e-122">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="43a2e-123">subscription</span><span class="sxs-lookup"><span data-stu-id="43a2e-123">subscription</span></span>](subscription.md) | <span data-ttu-id="43a2e-124">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="43a2e-124">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="43a2e-125">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="43a2e-125">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="43a2e-126">subscription</span><span class="sxs-lookup"><span data-stu-id="43a2e-126">subscription</span></span>](subscription.md) | <span data-ttu-id="43a2e-127">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="43a2e-127">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="43a2e-128">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="43a2e-128">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="43a2e-129">subscription</span><span class="sxs-lookup"><span data-stu-id="43a2e-129">subscription</span></span>](subscription.md) | <span data-ttu-id="43a2e-130">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="43a2e-130">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="43a2e-131">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="43a2e-131">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="43a2e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="43a2e-132">None</span></span> | <span data-ttu-id="43a2e-133">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="43a2e-133">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="43a2e-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="43a2e-134">Properties</span></span>

| <span data-ttu-id="43a2e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="43a2e-135">Property</span></span> | <span data-ttu-id="43a2e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="43a2e-136">Type</span></span> | <span data-ttu-id="43a2e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="43a2e-137">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="43a2e-138">changeType</span><span class="sxs-lookup"><span data-stu-id="43a2e-138">changeType</span></span> | <span data-ttu-id="43a2e-139">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-139">string</span></span> | <span data-ttu-id="43a2e-140">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="43a2e-140">Required.</span></span> <span data-ttu-id="43a2e-141">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="43a2e-141">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="43a2e-142">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="43a2e-142">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="43a2e-143">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="43a2e-143">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="43a2e-144">Примечание. Уведомления о корневых элементах диска и списках поддерживают только changeType `updated`.</span><span class="sxs-lookup"><span data-stu-id="43a2e-144">Note: Drive root item and list notifications support only the `updated` changeType.</span></span> <span data-ttu-id="43a2e-145">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="43a2e-145">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="43a2e-146">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="43a2e-146">notificationUrl</span></span> | <span data-ttu-id="43a2e-147">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-147">string</span></span> | <span data-ttu-id="43a2e-148">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="43a2e-148">Required.</span></span> <span data-ttu-id="43a2e-149">URL-адрес конечной точки, которая будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="43a2e-149">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="43a2e-150">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="43a2e-150">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="43a2e-151">resource</span><span class="sxs-lookup"><span data-stu-id="43a2e-151">resource</span></span> | <span data-ttu-id="43a2e-152">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-152">string</span></span> | <span data-ttu-id="43a2e-153">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="43a2e-153">Required.</span></span> <span data-ttu-id="43a2e-154">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="43a2e-154">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="43a2e-155">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="43a2e-155">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="43a2e-156">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="43a2e-156">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="43a2e-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43a2e-157">expirationDateTime</span></span> | [<span data-ttu-id="43a2e-158">dateTime</span><span class="sxs-lookup"><span data-stu-id="43a2e-158">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="43a2e-159">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="43a2e-159">Required.</span></span> <span data-ttu-id="43a2e-160">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="43a2e-160">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="43a2e-161">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="43a2e-161">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="43a2e-162">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="43a2e-162">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="43a2e-163">clientState</span><span class="sxs-lookup"><span data-stu-id="43a2e-163">clientState</span></span> | <span data-ttu-id="43a2e-164">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-164">string</span></span> | <span data-ttu-id="43a2e-165">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="43a2e-165">Optional.</span></span> <span data-ttu-id="43a2e-166">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="43a2e-166">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="43a2e-167">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="43a2e-167">The maximum length is 128 characters.</span></span> <span data-ttu-id="43a2e-168">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="43a2e-168">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="43a2e-169">id</span><span class="sxs-lookup"><span data-stu-id="43a2e-169">id</span></span> | <span data-ttu-id="43a2e-170">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-170">string</span></span> | <span data-ttu-id="43a2e-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43a2e-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="43a2e-173">applicationId</span><span class="sxs-lookup"><span data-stu-id="43a2e-173">applicationId</span></span> | <span data-ttu-id="43a2e-174">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-174">string</span></span> | <span data-ttu-id="43a2e-175">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="43a2e-175">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="43a2e-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43a2e-176">Read-only.</span></span> |
| <span data-ttu-id="43a2e-177">creatorId</span><span class="sxs-lookup"><span data-stu-id="43a2e-177">creatorId</span></span> | <span data-ttu-id="43a2e-178">string</span><span class="sxs-lookup"><span data-stu-id="43a2e-178">string</span></span> | <span data-ttu-id="43a2e-179">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="43a2e-179">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="43a2e-180">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="43a2e-180">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="43a2e-181">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="43a2e-181">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="43a2e-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43a2e-182">Read-only.</span></span> |
| <span data-ttu-id="43a2e-183">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="43a2e-183">latestSupportedTlsVersion</span></span> | <span data-ttu-id="43a2e-184">Строка</span><span class="sxs-lookup"><span data-stu-id="43a2e-184">String</span></span> | <span data-ttu-id="43a2e-185">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="43a2e-185">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="43a2e-186">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="43a2e-186">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="43a2e-187">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="43a2e-187">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="43a2e-188">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="43a2e-188">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="43a2e-189">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="43a2e-189">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="43a2e-190">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="43a2e-190">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="43a2e-191">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="43a2e-191">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="43a2e-192">Ресурс</span><span class="sxs-lookup"><span data-stu-id="43a2e-192">Resource</span></span>            | <span data-ttu-id="43a2e-193">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="43a2e-193">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="43a2e-194">Пользователь, группа, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="43a2e-194">User, group, other directory resources</span></span>   | <span data-ttu-id="43a2e-195">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-196">Почта</span><span class="sxs-lookup"><span data-stu-id="43a2e-196">Mail</span></span>                | <span data-ttu-id="43a2e-197">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-198">Календарь</span><span class="sxs-lookup"><span data-stu-id="43a2e-198">Calendar</span></span>            | <span data-ttu-id="43a2e-199">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-200">Контакты</span><span class="sxs-lookup"><span data-stu-id="43a2e-200">Contacts</span></span>            | <span data-ttu-id="43a2e-201">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-202">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="43a2e-202">Group conversations</span></span> | <span data-ttu-id="43a2e-203">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-203">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-204">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="43a2e-204">Drive root items</span></span>    | <span data-ttu-id="43a2e-205">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-205">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-206">Список SharePoint</span><span class="sxs-lookup"><span data-stu-id="43a2e-206">SharePoint list</span></span>     | <span data-ttu-id="43a2e-207">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-207">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="43a2e-208">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="43a2e-208">Security alerts</span></span>     | <span data-ttu-id="43a2e-209">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="43a2e-209">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="43a2e-210">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="43a2e-210">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="43a2e-211">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="43a2e-211">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="43a2e-212">Отношения</span><span class="sxs-lookup"><span data-stu-id="43a2e-212">Relationships</span></span>

<span data-ttu-id="43a2e-213">Нет</span><span class="sxs-lookup"><span data-stu-id="43a2e-213">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43a2e-214">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43a2e-214">JSON representation</span></span>

<span data-ttu-id="43a2e-215">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43a2e-215">Here is a JSON representation of the resource.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
