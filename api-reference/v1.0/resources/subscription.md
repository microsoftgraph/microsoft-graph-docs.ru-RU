---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 60219f50b78cf5c636fab1b24aa75922893002fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033972"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="0be2b-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="0be2b-104">subscription resource type</span></span>

<span data-ttu-id="0be2b-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0be2b-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="0be2b-106">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0be2b-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="0be2b-107">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="0be2b-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="0be2b-108">[Беседа][] группы Office 365</span><span class="sxs-lookup"><span data-stu-id="0be2b-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="0be2b-109">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="0be2b-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="0be2b-110">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0be2b-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="0be2b-111">[Оповещение][] из Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="0be2b-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="0be2b-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0be2b-112">JSON representation</span></span>

<span data-ttu-id="0be2b-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0be2b-113">Here is a JSON representation of the resource.</span></span>

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
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0be2b-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="0be2b-114">Properties</span></span>

| <span data-ttu-id="0be2b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0be2b-115">Property</span></span> | <span data-ttu-id="0be2b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="0be2b-116">Type</span></span> | <span data-ttu-id="0be2b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0be2b-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="0be2b-118">changeType</span><span class="sxs-lookup"><span data-stu-id="0be2b-118">changeType</span></span> | <span data-ttu-id="0be2b-119">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-119">string</span></span> | <span data-ttu-id="0be2b-120">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0be2b-120">Required.</span></span> <span data-ttu-id="0be2b-121">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="0be2b-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="0be2b-122">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="0be2b-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="0be2b-123">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="0be2b-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="0be2b-124">Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="0be2b-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="0be2b-125">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="0be2b-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="0be2b-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="0be2b-126">notificationUrl</span></span> | <span data-ttu-id="0be2b-127">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-127">string</span></span> | <span data-ttu-id="0be2b-128">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0be2b-128">Required.</span></span> <span data-ttu-id="0be2b-129">URL-адрес конечной точки, которая будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="0be2b-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="0be2b-130">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="0be2b-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="0be2b-131">resource</span><span class="sxs-lookup"><span data-stu-id="0be2b-131">resource</span></span> | <span data-ttu-id="0be2b-132">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-132">string</span></span> | <span data-ttu-id="0be2b-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0be2b-133">Required.</span></span> <span data-ttu-id="0be2b-134">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="0be2b-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="0be2b-135">Не включайте базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="0be2b-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="0be2b-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0be2b-136">expirationDateTime</span></span> | [<span data-ttu-id="0be2b-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="0be2b-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="0be2b-138">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0be2b-138">Required.</span></span> <span data-ttu-id="0be2b-139">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="0be2b-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="0be2b-140">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="0be2b-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="0be2b-141">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="0be2b-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="0be2b-142">clientState</span><span class="sxs-lookup"><span data-stu-id="0be2b-142">clientState</span></span> | <span data-ttu-id="0be2b-143">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-143">string</span></span> | <span data-ttu-id="0be2b-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0be2b-144">Optional.</span></span> <span data-ttu-id="0be2b-145">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="0be2b-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="0be2b-146">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="0be2b-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="0be2b-147">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="0be2b-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="0be2b-148">id</span><span class="sxs-lookup"><span data-stu-id="0be2b-148">id</span></span> | <span data-ttu-id="0be2b-149">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-149">string</span></span> | <span data-ttu-id="0be2b-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0be2b-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="0be2b-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="0be2b-152">applicationId</span></span> | <span data-ttu-id="0be2b-153">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-153">string</span></span> | <span data-ttu-id="0be2b-154">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="0be2b-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="0be2b-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0be2b-155">Read-only.</span></span> |
| <span data-ttu-id="0be2b-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="0be2b-156">creatorId</span></span> | <span data-ttu-id="0be2b-157">string</span><span class="sxs-lookup"><span data-stu-id="0be2b-157">string</span></span> | <span data-ttu-id="0be2b-158">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="0be2b-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="0be2b-159">Если в приложении использовались делегированные разрешения для создания подписки, это поле содержит идентификатор вошедшего пользователя, от имени которого вызвано приложение.</span><span class="sxs-lookup"><span data-stu-id="0be2b-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="0be2b-160">Если в приложении использовались разрешения для приложений, это поле содержит идентификатор субъекта-службы, соответствующей приложению.</span><span class="sxs-lookup"><span data-stu-id="0be2b-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="0be2b-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0be2b-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="0be2b-162">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="0be2b-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="0be2b-163">Ресурс</span><span class="sxs-lookup"><span data-stu-id="0be2b-163">Resource</span></span>            | <span data-ttu-id="0be2b-164">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="0be2b-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="0be2b-165">Пользователь, группа, другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="0be2b-165">User, group, other directory resources</span></span>   | <span data-ttu-id="0be2b-166">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-167">Почта</span><span class="sxs-lookup"><span data-stu-id="0be2b-167">Mail</span></span>                | <span data-ttu-id="0be2b-168">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-169">Календарь</span><span class="sxs-lookup"><span data-stu-id="0be2b-169">Calendar</span></span>            | <span data-ttu-id="0be2b-170">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-171">Контакты</span><span class="sxs-lookup"><span data-stu-id="0be2b-171">Contacts</span></span>            | <span data-ttu-id="0be2b-172">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-173">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="0be2b-173">Group conversations</span></span> | <span data-ttu-id="0be2b-174">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-175">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="0be2b-175">Drive root items</span></span>    | <span data-ttu-id="0be2b-176">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="0be2b-177">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="0be2b-177">Security alerts</span></span>     | <span data-ttu-id="0be2b-178">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="0be2b-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="0be2b-179">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="0be2b-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="0be2b-180">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="0be2b-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="0be2b-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="0be2b-181">Relationships</span></span>

<span data-ttu-id="0be2b-182">Нет</span><span class="sxs-lookup"><span data-stu-id="0be2b-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="0be2b-183">Методы</span><span class="sxs-lookup"><span data-stu-id="0be2b-183">Methods</span></span>

| <span data-ttu-id="0be2b-184">Метод</span><span class="sxs-lookup"><span data-stu-id="0be2b-184">Method</span></span> | <span data-ttu-id="0be2b-185">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0be2b-185">Return Type</span></span> | <span data-ttu-id="0be2b-186">Описание</span><span class="sxs-lookup"><span data-stu-id="0be2b-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="0be2b-187">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="0be2b-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="0be2b-188">subscription</span><span class="sxs-lookup"><span data-stu-id="0be2b-188">subscription</span></span>](subscription.md) | <span data-ttu-id="0be2b-189">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0be2b-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="0be2b-190">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="0be2b-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="0be2b-191">subscription</span><span class="sxs-lookup"><span data-stu-id="0be2b-191">subscription</span></span>](subscription.md) | <span data-ttu-id="0be2b-192">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="0be2b-192">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="0be2b-193">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="0be2b-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="0be2b-194">subscription</span><span class="sxs-lookup"><span data-stu-id="0be2b-194">subscription</span></span>](subscription.md) | <span data-ttu-id="0be2b-195">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="0be2b-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="0be2b-196">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="0be2b-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="0be2b-197">subscription</span><span class="sxs-lookup"><span data-stu-id="0be2b-197">subscription</span></span>](subscription.md) | <span data-ttu-id="0be2b-198">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="0be2b-198">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="0be2b-199">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="0be2b-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="0be2b-200">Нет</span><span class="sxs-lookup"><span data-stu-id="0be2b-200">None</span></span> |<span data-ttu-id="0be2b-201">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="0be2b-201">Deletes a subscription object.</span></span> |

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
