---
title: Тип ресурса Subscription
description: 'Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. В настоящее время подписки включены для следующих ресурсов:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163940"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="4a2ae-104">Тип ресурса Subscription</span><span class="sxs-lookup"><span data-stu-id="4a2ae-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2ae-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="4a2ae-106">В настоящее время подписки включены для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="4a2ae-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="4a2ae-107">[Сообщение][], [событие][]или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="4a2ae-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="4a2ae-108">[Беседа][] с группой Office 365</span><span class="sxs-lookup"><span data-stu-id="4a2ae-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="4a2ae-109">Контент в иерархии корневой папки [driveItem][] в Onedrive для бизнеса или корневой папки или вложенной папки [driveItem][] в личном OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="4a2ae-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="4a2ae-110">[Пользователь][] или [Группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4a2ae-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="4a2ae-111">[Оповещение][] из API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4a2ae-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="4a2ae-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a2ae-112">JSON representation</span></span>

<span data-ttu-id="4a2ae-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-113">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="4a2ae-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a2ae-114">Properties</span></span>

| <span data-ttu-id="4a2ae-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a2ae-115">Property</span></span> | <span data-ttu-id="4a2ae-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4a2ae-116">Type</span></span> | <span data-ttu-id="4a2ae-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4a2ae-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4a2ae-118">changeType</span><span class="sxs-lookup"><span data-stu-id="4a2ae-118">changeType</span></span> | <span data-ttu-id="4a2ae-119">строка</span><span class="sxs-lookup"><span data-stu-id="4a2ae-119">string</span></span> | <span data-ttu-id="4a2ae-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-120">Required.</span></span> <span data-ttu-id="4a2ae-121">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="4a2ae-122">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="4a2ae-123">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="4a2ae-124">Note: уведомления корневого элемента диска поддерживают только `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="4a2ae-125">Поддержка `updated` и `deleted` ChangeType уведомлений для пользователей и групп.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="4a2ae-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="4a2ae-126">notificationUrl</span></span> | <span data-ttu-id="4a2ae-127">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-127">string</span></span> | <span data-ttu-id="4a2ae-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-128">Required.</span></span> <span data-ttu-id="4a2ae-129">URL-адрес конечной точки, которая будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="4a2ae-130">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="4a2ae-131">resource</span><span class="sxs-lookup"><span data-stu-id="4a2ae-131">resource</span></span> | <span data-ttu-id="4a2ae-132">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-132">string</span></span> | <span data-ttu-id="4a2ae-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-133">Required.</span></span> <span data-ttu-id="4a2ae-134">Указывает ресурс, для которого будет выполняться отслеживание изменений.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="4a2ae-135">Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="4a2ae-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="4a2ae-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4a2ae-136">expirationDateTime</span></span> | <span data-ttu-id="4a2ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a2ae-137">DateTimeOffset</span></span> | <span data-ttu-id="4a2ae-138">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-138">Required.</span></span> <span data-ttu-id="4a2ae-139">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="4a2ae-140">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="4a2ae-141">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="4a2ae-142">clientState</span><span class="sxs-lookup"><span data-stu-id="4a2ae-142">clientState</span></span> | <span data-ttu-id="4a2ae-143">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-143">string</span></span> | <span data-ttu-id="4a2ae-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-144">Optional.</span></span> <span data-ttu-id="4a2ae-145">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="4a2ae-146">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="4a2ae-147">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="4a2ae-148">id</span><span class="sxs-lookup"><span data-stu-id="4a2ae-148">id</span></span> | <span data-ttu-id="4a2ae-149">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-149">string</span></span> | <span data-ttu-id="4a2ae-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="4a2ae-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="4a2ae-152">applicationId</span></span> | <span data-ttu-id="4a2ae-153">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-153">string</span></span> | <span data-ttu-id="4a2ae-154">Идентификатор приложения, используемого для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="4a2ae-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-155">Read-only.</span></span> |
| <span data-ttu-id="4a2ae-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="4a2ae-156">creatorId</span></span> | <span data-ttu-id="4a2ae-157">string</span><span class="sxs-lookup"><span data-stu-id="4a2ae-157">string</span></span> | <span data-ttu-id="4a2ae-158">Идентификатор пользователя или участника службы, который создал подписку.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="4a2ae-159">Если приложение использовало делегированные разрешения для создания подписки, это поле содержит идентификатор пользователя, выполнившего вход в систему, вызываемую приложением от имени.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="4a2ae-160">Если приложение использовало разрешения приложения, это поле содержит идентификатор участника службы, соответствующего приложению.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="4a2ae-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="4a2ae-162">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="4a2ae-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="4a2ae-163">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a2ae-163">Resource</span></span>            | <span data-ttu-id="4a2ae-164">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="4a2ae-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="4a2ae-165">Почта</span><span class="sxs-lookup"><span data-stu-id="4a2ae-165">Mail</span></span>                | <span data-ttu-id="4a2ae-166">4230 минут (в течение 3 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4a2ae-167">Календарь</span><span class="sxs-lookup"><span data-stu-id="4a2ae-167">Calendar</span></span>            | <span data-ttu-id="4a2ae-168">4230 минут (в течение 3 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4a2ae-169">Контакты</span><span class="sxs-lookup"><span data-stu-id="4a2ae-169">Contacts</span></span>            | <span data-ttu-id="4a2ae-170">4230 минут (в течение 3 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4a2ae-171">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="4a2ae-171">Group conversations</span></span> | <span data-ttu-id="4a2ae-172">4230 минут (в течение 3 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4a2ae-173">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="4a2ae-173">Drive root items</span></span>    | <span data-ttu-id="4a2ae-174">4230 минут (в течение 3 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4a2ae-175">Оповещения системы безопасности</span><span class="sxs-lookup"><span data-stu-id="4a2ae-175">Security alerts</span></span>     | <span data-ttu-id="4a2ae-176">43200 минут (30 дней)</span><span class="sxs-lookup"><span data-stu-id="4a2ae-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="4a2ae-177">**Примечание:** Существующие приложения и новые приложения не должны превышать поддерживаемое значение.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="4a2ae-178">В будущем все запросы на создание или продление подписки, превышающие максимальное значение, завершатся неудачей.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="4a2ae-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="4a2ae-179">Relationships</span></span>

<span data-ttu-id="4a2ae-180">Нет</span><span class="sxs-lookup"><span data-stu-id="4a2ae-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="4a2ae-181">Методы</span><span class="sxs-lookup"><span data-stu-id="4a2ae-181">Methods</span></span>

| <span data-ttu-id="4a2ae-182">Метод</span><span class="sxs-lookup"><span data-stu-id="4a2ae-182">Method</span></span> | <span data-ttu-id="4a2ae-183">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4a2ae-183">Return Type</span></span> | <span data-ttu-id="4a2ae-184">Описание</span><span class="sxs-lookup"><span data-stu-id="4a2ae-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="4a2ae-185">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="4a2ae-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="4a2ae-186">subscription</span><span class="sxs-lookup"><span data-stu-id="4a2ae-186">subscription</span></span>](subscription.md) | <span data-ttu-id="4a2ae-187">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="4a2ae-188">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="4a2ae-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="4a2ae-189">subscription</span><span class="sxs-lookup"><span data-stu-id="4a2ae-189">subscription</span></span>](subscription.md) | <span data-ttu-id="4a2ae-190">Продлить подписку, обновив срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="4a2ae-191">Список подписок</span><span class="sxs-lookup"><span data-stu-id="4a2ae-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="4a2ae-192">subscription</span><span class="sxs-lookup"><span data-stu-id="4a2ae-192">subscription</span></span>](subscription.md) | <span data-ttu-id="4a2ae-193">Список активных подписок.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="4a2ae-194">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="4a2ae-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="4a2ae-195">subscription</span><span class="sxs-lookup"><span data-stu-id="4a2ae-195">subscription</span></span>](subscription.md) | <span data-ttu-id="4a2ae-196">Чтение свойств и связей объекта Subscription.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="4a2ae-197">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="4a2ae-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="4a2ae-198">Нет</span><span class="sxs-lookup"><span data-stu-id="4a2ae-198">None</span></span> | <span data-ttu-id="4a2ae-199">Удаление объекта подписки.</span><span class="sxs-lookup"><span data-stu-id="4a2ae-199">Delete a subscription object.</span></span> |

[контакт]: ./contact.md
[contact]: ./contact.md
[беседа]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[акций]: ./alert.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
