---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 563d232d200797b87e894292e31eb48ad88bf540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342914"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="1bd3c-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="1bd3c-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bd3c-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="1bd3c-106">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="1bd3c-107">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="1bd3c-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="1bd3c-108">[Беседа][] группы Office 365</span><span class="sxs-lookup"><span data-stu-id="1bd3c-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="1bd3c-109">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="1bd3c-110">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1bd3c-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="1bd3c-111">[Оповещение][] из Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="1bd3c-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="1bd3c-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bd3c-112">JSON representation</span></span>

<span data-ttu-id="1bd3c-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
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
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1bd3c-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bd3c-114">Properties</span></span>

| <span data-ttu-id="1bd3c-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bd3c-115">Property</span></span> | <span data-ttu-id="1bd3c-116">Тип</span><span class="sxs-lookup"><span data-stu-id="1bd3c-116">Type</span></span> | <span data-ttu-id="1bd3c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd3c-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1bd3c-118">changeType</span><span class="sxs-lookup"><span data-stu-id="1bd3c-118">changeType</span></span> | <span data-ttu-id="1bd3c-119">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-119">string</span></span> | <span data-ttu-id="1bd3c-120">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-120">Required.</span></span> <span data-ttu-id="1bd3c-121">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="1bd3c-122">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="1bd3c-123">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="1bd3c-124">Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="1bd3c-125">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="1bd3c-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="1bd3c-126">notificationUrl</span></span> | <span data-ttu-id="1bd3c-127">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-127">string</span></span> | <span data-ttu-id="1bd3c-128">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-128">Required.</span></span> <span data-ttu-id="1bd3c-129">URL-адрес конечной точки, принимающей уведомления.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-129">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="1bd3c-130">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="1bd3c-131">Лифецикленотификатионурл</span><span class="sxs-lookup"><span data-stu-id="1bd3c-131">lifecycleNotificationUrl</span></span> | <span data-ttu-id="1bd3c-132">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-132">string</span></span> | <span data-ttu-id="1bd3c-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-133">Optional.</span></span> <span data-ttu-id="1bd3c-134">URL-адрес конечной точки, которая получает уведомления жизненного `subscriptionRemoved` цикла `missed` , включая и уведомления.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-134">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="1bd3c-135">Если этот параметр не указан, уведомления будут доставляться в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-135">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="1bd3c-136">[Узнайте больше](/graph/webhooks-outlook-authz.md) о том, как ресурсы Outlook используют Уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-136">[Read more](/graph/webhooks-outlook-authz.md) about how Outlook resources use lifecycle notifications.</span></span>  <span data-ttu-id="1bd3c-137">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-137">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="1bd3c-138">resource</span><span class="sxs-lookup"><span data-stu-id="1bd3c-138">resource</span></span> | <span data-ttu-id="1bd3c-139">строка</span><span class="sxs-lookup"><span data-stu-id="1bd3c-139">string</span></span> | <span data-ttu-id="1bd3c-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-140">Required.</span></span> <span data-ttu-id="1bd3c-141">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-141">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1bd3c-142">Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="1bd3c-142">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="1bd3c-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1bd3c-143">expirationDateTime</span></span> | <span data-ttu-id="1bd3c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bd3c-144">DateTimeOffset</span></span> | <span data-ttu-id="1bd3c-145">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-145">Required.</span></span> <span data-ttu-id="1bd3c-146">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-146">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="1bd3c-147">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-147">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="1bd3c-148">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-148">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="1bd3c-149">clientState</span><span class="sxs-lookup"><span data-stu-id="1bd3c-149">clientState</span></span> | <span data-ttu-id="1bd3c-150">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-150">string</span></span> | <span data-ttu-id="1bd3c-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-151">Optional.</span></span> <span data-ttu-id="1bd3c-152">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-152">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="1bd3c-153">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-153">The maximum length is 255 characters.</span></span> <span data-ttu-id="1bd3c-154">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-154">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="1bd3c-155">id</span><span class="sxs-lookup"><span data-stu-id="1bd3c-155">id</span></span> | <span data-ttu-id="1bd3c-156">строка</span><span class="sxs-lookup"><span data-stu-id="1bd3c-156">string</span></span> | <span data-ttu-id="1bd3c-p110">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="1bd3c-159">applicationId</span><span class="sxs-lookup"><span data-stu-id="1bd3c-159">applicationId</span></span> | <span data-ttu-id="1bd3c-160">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-160">string</span></span> | <span data-ttu-id="1bd3c-161">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-161">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="1bd3c-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-162">Read-only.</span></span> |
| <span data-ttu-id="1bd3c-163">creatorId</span><span class="sxs-lookup"><span data-stu-id="1bd3c-163">creatorId</span></span> | <span data-ttu-id="1bd3c-164">string</span><span class="sxs-lookup"><span data-stu-id="1bd3c-164">string</span></span> | <span data-ttu-id="1bd3c-165">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-165">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="1bd3c-166">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-166">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="1bd3c-167">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-167">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="1bd3c-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-168">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="1bd3c-169">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="1bd3c-169">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="1bd3c-170">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1bd3c-170">Resource</span></span>            | <span data-ttu-id="1bd3c-171">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="1bd3c-171">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="1bd3c-172">Почта</span><span class="sxs-lookup"><span data-stu-id="1bd3c-172">Mail</span></span>                | <span data-ttu-id="1bd3c-173">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-173">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1bd3c-174">Календарь</span><span class="sxs-lookup"><span data-stu-id="1bd3c-174">Calendar</span></span>            | <span data-ttu-id="1bd3c-175">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-175">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1bd3c-176">Контакты</span><span class="sxs-lookup"><span data-stu-id="1bd3c-176">Contacts</span></span>            | <span data-ttu-id="1bd3c-177">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-177">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1bd3c-178">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="1bd3c-178">Group conversations</span></span> | <span data-ttu-id="1bd3c-179">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-179">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1bd3c-180">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="1bd3c-180">Drive root items</span></span>    | <span data-ttu-id="1bd3c-181">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-181">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1bd3c-182">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="1bd3c-182">Security alerts</span></span>     | <span data-ttu-id="1bd3c-183">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="1bd3c-183">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="1bd3c-184">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-184">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="1bd3c-185">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-185">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="1bd3c-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="1bd3c-186">Relationships</span></span>

<span data-ttu-id="1bd3c-187">Нет</span><span class="sxs-lookup"><span data-stu-id="1bd3c-187">None</span></span>

## <a name="methods"></a><span data-ttu-id="1bd3c-188">Методы</span><span class="sxs-lookup"><span data-stu-id="1bd3c-188">Methods</span></span>

| <span data-ttu-id="1bd3c-189">Метод</span><span class="sxs-lookup"><span data-stu-id="1bd3c-189">Method</span></span> | <span data-ttu-id="1bd3c-190">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1bd3c-190">Return Type</span></span> | <span data-ttu-id="1bd3c-191">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd3c-191">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="1bd3c-192">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1bd3c-192">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="1bd3c-193">subscription</span><span class="sxs-lookup"><span data-stu-id="1bd3c-193">subscription</span></span>](subscription.md) | <span data-ttu-id="1bd3c-194">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-194">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="1bd3c-195">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="1bd3c-195">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="1bd3c-196">subscription</span><span class="sxs-lookup"><span data-stu-id="1bd3c-196">subscription</span></span>](subscription.md) | <span data-ttu-id="1bd3c-197">Продлить подписку, обновив срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-197">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="1bd3c-198">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="1bd3c-198">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="1bd3c-199">subscription</span><span class="sxs-lookup"><span data-stu-id="1bd3c-199">subscription</span></span>](subscription.md) | <span data-ttu-id="1bd3c-200">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-200">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="1bd3c-201">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="1bd3c-201">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="1bd3c-202">subscription</span><span class="sxs-lookup"><span data-stu-id="1bd3c-202">subscription</span></span>](subscription.md) | <span data-ttu-id="1bd3c-203">Чтение свойств и связей объекта Subscription.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-203">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="1bd3c-204">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="1bd3c-204">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="1bd3c-205">Нет</span><span class="sxs-lookup"><span data-stu-id="1bd3c-205">None</span></span> | <span data-ttu-id="1bd3c-206">Удаление объекта подписки.</span><span class="sxs-lookup"><span data-stu-id="1bd3c-206">Delete a subscription object.</span></span> |

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
