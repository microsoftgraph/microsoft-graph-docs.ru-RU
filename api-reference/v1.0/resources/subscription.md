---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e036c357d65c7f01c1596095569f8dfe5b863007
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219673"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="96c53-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="96c53-104">subscription resource type</span></span>

<span data-ttu-id="96c53-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96c53-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="96c53-106">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="96c53-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="96c53-107">[Оповещение][] Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="96c53-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="96c53-108">[Беседа][] в группе Office 365</span><span class="sxs-lookup"><span data-stu-id="96c53-108">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="96c53-109">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="96c53-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="96c53-110">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="96c53-110">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="96c53-111">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="96c53-111">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="96c53-112">Сведения о возможных значениях пути к ресурсу для всех поддерживаемых ресурсов см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="96c53-112">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="96c53-113">Методы</span><span class="sxs-lookup"><span data-stu-id="96c53-113">Methods</span></span>

| <span data-ttu-id="96c53-114">Метод</span><span class="sxs-lookup"><span data-stu-id="96c53-114">Method</span></span> | <span data-ttu-id="96c53-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96c53-115">Return Type</span></span> | <span data-ttu-id="96c53-116">Описание</span><span class="sxs-lookup"><span data-stu-id="96c53-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="96c53-117">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="96c53-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="96c53-118">subscription</span><span class="sxs-lookup"><span data-stu-id="96c53-118">subscription</span></span>](subscription.md) | <span data-ttu-id="96c53-119">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96c53-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="96c53-120">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="96c53-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="96c53-121">subscription</span><span class="sxs-lookup"><span data-stu-id="96c53-121">subscription</span></span>](subscription.md) | <span data-ttu-id="96c53-122">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="96c53-122">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="96c53-123">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="96c53-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="96c53-124">subscription</span><span class="sxs-lookup"><span data-stu-id="96c53-124">subscription</span></span>](subscription.md) | <span data-ttu-id="96c53-125">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="96c53-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="96c53-126">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="96c53-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="96c53-127">subscription</span><span class="sxs-lookup"><span data-stu-id="96c53-127">subscription</span></span>](subscription.md) | <span data-ttu-id="96c53-128">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="96c53-128">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="96c53-129">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="96c53-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="96c53-130">Нет</span><span class="sxs-lookup"><span data-stu-id="96c53-130">None</span></span> | <span data-ttu-id="96c53-131">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="96c53-131">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96c53-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="96c53-132">Properties</span></span>

| <span data-ttu-id="96c53-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="96c53-133">Property</span></span> | <span data-ttu-id="96c53-134">Тип</span><span class="sxs-lookup"><span data-stu-id="96c53-134">Type</span></span> | <span data-ttu-id="96c53-135">Описание</span><span class="sxs-lookup"><span data-stu-id="96c53-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="96c53-136">changeType</span><span class="sxs-lookup"><span data-stu-id="96c53-136">changeType</span></span> | <span data-ttu-id="96c53-137">string</span><span class="sxs-lookup"><span data-stu-id="96c53-137">string</span></span> | <span data-ttu-id="96c53-138">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="96c53-138">Required.</span></span> <span data-ttu-id="96c53-139">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="96c53-139">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="96c53-140">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="96c53-140">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="96c53-141">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="96c53-141">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="96c53-142">Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="96c53-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="96c53-143">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="96c53-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="96c53-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="96c53-144">notificationUrl</span></span> | <span data-ttu-id="96c53-145">string</span><span class="sxs-lookup"><span data-stu-id="96c53-145">string</span></span> | <span data-ttu-id="96c53-146">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="96c53-146">Required.</span></span> <span data-ttu-id="96c53-147">URL-адрес конечной точки, которая будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="96c53-147">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="96c53-148">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="96c53-148">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="96c53-149">resource</span><span class="sxs-lookup"><span data-stu-id="96c53-149">resource</span></span> | <span data-ttu-id="96c53-150">string</span><span class="sxs-lookup"><span data-stu-id="96c53-150">string</span></span> | <span data-ttu-id="96c53-151">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="96c53-151">Required.</span></span> <span data-ttu-id="96c53-152">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="96c53-152">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="96c53-153">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="96c53-153">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="96c53-154">См. возможные [значения](webhooks.md) пути к ресурсу для всех поддерживаемых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="96c53-154">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="96c53-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="96c53-155">expirationDateTime</span></span> | [<span data-ttu-id="96c53-156">dateTime</span><span class="sxs-lookup"><span data-stu-id="96c53-156">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="96c53-157">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="96c53-157">Required.</span></span> <span data-ttu-id="96c53-158">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="96c53-158">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="96c53-159">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="96c53-159">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="96c53-160">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="96c53-160">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="96c53-161">clientState</span><span class="sxs-lookup"><span data-stu-id="96c53-161">clientState</span></span> | <span data-ttu-id="96c53-162">string</span><span class="sxs-lookup"><span data-stu-id="96c53-162">string</span></span> | <span data-ttu-id="96c53-163">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="96c53-163">Optional.</span></span> <span data-ttu-id="96c53-164">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="96c53-164">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="96c53-165">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="96c53-165">The maximum length is 128 characters.</span></span> <span data-ttu-id="96c53-166">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="96c53-166">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="96c53-167">id</span><span class="sxs-lookup"><span data-stu-id="96c53-167">id</span></span> | <span data-ttu-id="96c53-168">string</span><span class="sxs-lookup"><span data-stu-id="96c53-168">string</span></span> | <span data-ttu-id="96c53-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96c53-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="96c53-171">applicationId</span><span class="sxs-lookup"><span data-stu-id="96c53-171">applicationId</span></span> | <span data-ttu-id="96c53-172">string</span><span class="sxs-lookup"><span data-stu-id="96c53-172">string</span></span> | <span data-ttu-id="96c53-173">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="96c53-173">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="96c53-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96c53-174">Read-only.</span></span> |
| <span data-ttu-id="96c53-175">creatorId</span><span class="sxs-lookup"><span data-stu-id="96c53-175">creatorId</span></span> | <span data-ttu-id="96c53-176">string</span><span class="sxs-lookup"><span data-stu-id="96c53-176">string</span></span> | <span data-ttu-id="96c53-177">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="96c53-177">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="96c53-178">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="96c53-178">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="96c53-179">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="96c53-179">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="96c53-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96c53-180">Read-only.</span></span> |
| <span data-ttu-id="96c53-181">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="96c53-181">latestSupportedTlsVersion</span></span> | <span data-ttu-id="96c53-182">Строка</span><span class="sxs-lookup"><span data-stu-id="96c53-182">String</span></span> | <span data-ttu-id="96c53-183">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="96c53-183">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="96c53-184">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="96c53-184">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="96c53-185">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="96c53-185">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="96c53-186">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="96c53-186">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="96c53-187">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="96c53-187">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="96c53-188">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="96c53-188">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="96c53-189">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="96c53-189">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="96c53-190">Ресурс</span><span class="sxs-lookup"><span data-stu-id="96c53-190">Resource</span></span>            | <span data-ttu-id="96c53-191">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="96c53-191">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="96c53-192">Пользователь, группа, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="96c53-192">User, group, other directory resources</span></span>   | <span data-ttu-id="96c53-193">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-193">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-194">Почта</span><span class="sxs-lookup"><span data-stu-id="96c53-194">Mail</span></span>                | <span data-ttu-id="96c53-195">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-196">Календарь</span><span class="sxs-lookup"><span data-stu-id="96c53-196">Calendar</span></span>            | <span data-ttu-id="96c53-197">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-198">Контакты</span><span class="sxs-lookup"><span data-stu-id="96c53-198">Contacts</span></span>            | <span data-ttu-id="96c53-199">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-200">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="96c53-200">Group conversations</span></span> | <span data-ttu-id="96c53-201">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-202">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="96c53-202">Drive root items</span></span>    | <span data-ttu-id="96c53-203">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-203">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="96c53-204">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="96c53-204">Security alerts</span></span>     | <span data-ttu-id="96c53-205">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="96c53-205">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="96c53-206">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="96c53-206">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="96c53-207">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="96c53-207">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="96c53-208">Отношения</span><span class="sxs-lookup"><span data-stu-id="96c53-208">Relationships</span></span>

<span data-ttu-id="96c53-209">Нет</span><span class="sxs-lookup"><span data-stu-id="96c53-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c53-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96c53-210">JSON representation</span></span>

<span data-ttu-id="96c53-211">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96c53-211">Here is a JSON representation of the resource.</span></span>

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
