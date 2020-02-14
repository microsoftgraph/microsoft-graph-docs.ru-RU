---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 02f06d9de4a3e40c06208502b8b08fbc2ab06bd2
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953594"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="bcd1a-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="bcd1a-104">subscription resource type</span></span>

<span data-ttu-id="bcd1a-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="bcd1a-106">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="bcd1a-107">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="bcd1a-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="bcd1a-108">[Беседа][] группы Office 365</span><span class="sxs-lookup"><span data-stu-id="bcd1a-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="bcd1a-109">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="bcd1a-110">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bcd1a-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="bcd1a-111">[Оповещение][] из Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="bcd1a-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="methods"></a><span data-ttu-id="bcd1a-112">Методы</span><span class="sxs-lookup"><span data-stu-id="bcd1a-112">Methods</span></span>

| <span data-ttu-id="bcd1a-113">Метод</span><span class="sxs-lookup"><span data-stu-id="bcd1a-113">Method</span></span> | <span data-ttu-id="bcd1a-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bcd1a-114">Return Type</span></span> | <span data-ttu-id="bcd1a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="bcd1a-115">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="bcd1a-116">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="bcd1a-116">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="bcd1a-117">subscription</span><span class="sxs-lookup"><span data-stu-id="bcd1a-117">subscription</span></span>](subscription.md) | <span data-ttu-id="bcd1a-118">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-118">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="bcd1a-119">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="bcd1a-119">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="bcd1a-120">subscription</span><span class="sxs-lookup"><span data-stu-id="bcd1a-120">subscription</span></span>](subscription.md) | <span data-ttu-id="bcd1a-121">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-121">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="bcd1a-122">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="bcd1a-122">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="bcd1a-123">subscription</span><span class="sxs-lookup"><span data-stu-id="bcd1a-123">subscription</span></span>](subscription.md) | <span data-ttu-id="bcd1a-124">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-124">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="bcd1a-125">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="bcd1a-125">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="bcd1a-126">subscription</span><span class="sxs-lookup"><span data-stu-id="bcd1a-126">subscription</span></span>](subscription.md) | <span data-ttu-id="bcd1a-127">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-127">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="bcd1a-128">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="bcd1a-128">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="bcd1a-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bcd1a-129">None</span></span> | <span data-ttu-id="bcd1a-130">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-130">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bcd1a-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcd1a-131">Properties</span></span>

| <span data-ttu-id="bcd1a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcd1a-132">Property</span></span> | <span data-ttu-id="bcd1a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bcd1a-133">Type</span></span> | <span data-ttu-id="bcd1a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bcd1a-134">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="bcd1a-135">changeType</span><span class="sxs-lookup"><span data-stu-id="bcd1a-135">changeType</span></span> | <span data-ttu-id="bcd1a-136">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-136">string</span></span> | <span data-ttu-id="bcd1a-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-137">Required.</span></span> <span data-ttu-id="bcd1a-138">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="bcd1a-139">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="bcd1a-140">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-140">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="bcd1a-141">Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-141">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="bcd1a-142">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-142">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="bcd1a-143">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="bcd1a-143">notificationUrl</span></span> | <span data-ttu-id="bcd1a-144">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-144">string</span></span> | <span data-ttu-id="bcd1a-145">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-145">Required.</span></span> <span data-ttu-id="bcd1a-146">URL-адрес конечной точки, которая будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-146">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="bcd1a-147">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-147">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="bcd1a-148">resource</span><span class="sxs-lookup"><span data-stu-id="bcd1a-148">resource</span></span> | <span data-ttu-id="bcd1a-149">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-149">string</span></span> | <span data-ttu-id="bcd1a-150">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-150">Required.</span></span> <span data-ttu-id="bcd1a-151">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-151">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="bcd1a-152">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="bcd1a-152">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="bcd1a-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bcd1a-153">expirationDateTime</span></span> | [<span data-ttu-id="bcd1a-154">dateTime</span><span class="sxs-lookup"><span data-stu-id="bcd1a-154">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="bcd1a-155">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-155">Required.</span></span> <span data-ttu-id="bcd1a-156">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-156">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="bcd1a-157">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-157">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="bcd1a-158">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-158">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="bcd1a-159">clientState</span><span class="sxs-lookup"><span data-stu-id="bcd1a-159">clientState</span></span> | <span data-ttu-id="bcd1a-160">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-160">string</span></span> | <span data-ttu-id="bcd1a-161">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-161">Optional.</span></span> <span data-ttu-id="bcd1a-162">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-162">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="bcd1a-163">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-163">The maximum length is 128 characters.</span></span> <span data-ttu-id="bcd1a-164">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-164">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="bcd1a-165">id</span><span class="sxs-lookup"><span data-stu-id="bcd1a-165">id</span></span> | <span data-ttu-id="bcd1a-166">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-166">string</span></span> | <span data-ttu-id="bcd1a-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="bcd1a-169">applicationId</span><span class="sxs-lookup"><span data-stu-id="bcd1a-169">applicationId</span></span> | <span data-ttu-id="bcd1a-170">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-170">string</span></span> | <span data-ttu-id="bcd1a-171">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-171">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="bcd1a-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-172">Read-only.</span></span> |
| <span data-ttu-id="bcd1a-173">creatorId</span><span class="sxs-lookup"><span data-stu-id="bcd1a-173">creatorId</span></span> | <span data-ttu-id="bcd1a-174">string</span><span class="sxs-lookup"><span data-stu-id="bcd1a-174">string</span></span> | <span data-ttu-id="bcd1a-175">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-175">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="bcd1a-176">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-176">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="bcd1a-177">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-177">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="bcd1a-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-178">Read-only.</span></span> |
| <span data-ttu-id="bcd1a-179">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="bcd1a-179">latestSupportedTlsVersion</span></span> | <span data-ttu-id="bcd1a-180">Строка</span><span class="sxs-lookup"><span data-stu-id="bcd1a-180">String</span></span> | <span data-ttu-id="bcd1a-181">Указывает последнюю версию протокола TLS, поддерживаемую конечной точкой уведомлений, указанной с помощью свойства **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-181">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="bcd1a-182">Допустимые значения: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-182">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="bcd1a-183">Для подписчиков, чья конечная точка уведомлений поддерживает более раннюю версию, чем рекомендуемая в настоящее время (TLS 1.2), указание этого свойства в установленные [сроки](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) позволит им временно применять устаревшую версию TLS до перехода на TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-183">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="bcd1a-184">Если такие подписчики не настроят это свойство согласно соответствующим срокам, действия с подпиской будут завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-184">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="bcd1a-185">Для подписчиков, чья конечная точка уведомлений уже поддерживает TLS 1.2, настройка этого свойства необязательна.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-185">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="bcd1a-186">В таких случаях Microsoft Graph по умолчанию присваивает свойству значение `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-186">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="bcd1a-187">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="bcd1a-187">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="bcd1a-188">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bcd1a-188">Resource</span></span>            | <span data-ttu-id="bcd1a-189">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="bcd1a-189">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="bcd1a-190">Пользователь, группа, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="bcd1a-190">User, group, other directory resources</span></span>   | <span data-ttu-id="bcd1a-191">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-191">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-192">Почта</span><span class="sxs-lookup"><span data-stu-id="bcd1a-192">Mail</span></span>                | <span data-ttu-id="bcd1a-193">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-193">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-194">Календарь</span><span class="sxs-lookup"><span data-stu-id="bcd1a-194">Calendar</span></span>            | <span data-ttu-id="bcd1a-195">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-196">Контакты</span><span class="sxs-lookup"><span data-stu-id="bcd1a-196">Contacts</span></span>            | <span data-ttu-id="bcd1a-197">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-198">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="bcd1a-198">Group conversations</span></span> | <span data-ttu-id="bcd1a-199">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-200">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="bcd1a-200">Drive root items</span></span>    | <span data-ttu-id="bcd1a-201">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bcd1a-202">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="bcd1a-202">Security alerts</span></span>     | <span data-ttu-id="bcd1a-203">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="bcd1a-203">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="bcd1a-204">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-204">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="bcd1a-205">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-205">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="bcd1a-206">Отношения</span><span class="sxs-lookup"><span data-stu-id="bcd1a-206">Relationships</span></span>

<span data-ttu-id="bcd1a-207">Нет</span><span class="sxs-lookup"><span data-stu-id="bcd1a-207">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcd1a-208">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcd1a-208">JSON representation</span></span>

<span data-ttu-id="bcd1a-209">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcd1a-209">Here is a JSON representation of the resource.</span></span>

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
