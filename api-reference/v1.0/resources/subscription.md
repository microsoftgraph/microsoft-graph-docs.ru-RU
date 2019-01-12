---
title: Тип ресурса подписки
description: 'Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены следующие ресурсы:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7837524f2ce20a24154b84a82537ec6a4149bfe9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917820"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="bb1ad-104">Тип ресурса подписки</span><span class="sxs-lookup"><span data-stu-id="bb1ad-104">subscription resource type</span></span>

<span data-ttu-id="bb1ad-105">Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="bb1ad-106">На данный момент подписки включены следующие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="bb1ad-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="bb1ad-107">Почты, события и контакты из Outlook.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="bb1ad-108">Беседы в группах Office.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="bb1ad-109">Диск корневым элементов из службы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="bb1ad-110">Пользователи и группы из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="bb1ad-111">Оповещения о от безопасности Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb1ad-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb1ad-112">JSON representation</span></span>

<span data-ttu-id="bb1ad-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bb1ad-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb1ad-114">Properties</span></span>

| <span data-ttu-id="bb1ad-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb1ad-115">Property</span></span> | <span data-ttu-id="bb1ad-116">Тип</span><span class="sxs-lookup"><span data-stu-id="bb1ad-116">Type</span></span> | <span data-ttu-id="bb1ad-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bb1ad-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="bb1ad-118">changeType</span><span class="sxs-lookup"><span data-stu-id="bb1ad-118">changeType</span></span> | <span data-ttu-id="bb1ad-119">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-119">string</span></span> | <span data-ttu-id="bb1ad-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-120">Required.</span></span> <span data-ttu-id="bb1ad-121">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="bb1ad-122">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="bb1ad-123">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="bb1ad-124">Примечание: Диск корневого элемента уведомлений поддерживает только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="bb1ad-125">Уведомления пользователей и групп поддержки `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="bb1ad-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="bb1ad-126">notificationUrl</span></span> | <span data-ttu-id="bb1ad-127">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-127">string</span></span> | <span data-ttu-id="bb1ad-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-128">Required.</span></span> <span data-ttu-id="bb1ad-129">URL-адрес конечной точки, который будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="bb1ad-130">Этот URL-адрес необходимо использовать протокол HTTPS протокола.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="bb1ad-131">resource</span><span class="sxs-lookup"><span data-stu-id="bb1ad-131">resource</span></span> | <span data-ttu-id="bb1ad-132">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-132">string</span></span> | <span data-ttu-id="bb1ad-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-133">Required.</span></span> <span data-ttu-id="bb1ad-134">Указывает ресурс, к которому будет выполняться мониторинг изменений.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="bb1ad-135">Не включать базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="bb1ad-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="bb1ad-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb1ad-136">expirationDateTime</span></span> | [<span data-ttu-id="bb1ad-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="bb1ad-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="bb1ad-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-138">Required.</span></span> <span data-ttu-id="bb1ad-139">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="bb1ad-140">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="bb1ad-141">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="bb1ad-142">clientState</span><span class="sxs-lookup"><span data-stu-id="bb1ad-142">clientState</span></span> | <span data-ttu-id="bb1ad-143">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-143">string</span></span> | <span data-ttu-id="bb1ad-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-144">Optional.</span></span> <span data-ttu-id="bb1ad-145">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="bb1ad-146">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="bb1ad-147">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="bb1ad-148">id</span><span class="sxs-lookup"><span data-stu-id="bb1ad-148">id</span></span> | <span data-ttu-id="bb1ad-149">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-149">string</span></span> | <span data-ttu-id="bb1ad-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="bb1ad-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="bb1ad-152">applicationId</span></span> | <span data-ttu-id="bb1ad-153">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-153">string</span></span> | <span data-ttu-id="bb1ad-154">Идентификатор приложения, используемого для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="bb1ad-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-155">Read-only.</span></span> |
| <span data-ttu-id="bb1ad-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="bb1ad-156">creatorId</span></span> | <span data-ttu-id="bb1ad-157">строка</span><span class="sxs-lookup"><span data-stu-id="bb1ad-157">string</span></span> | <span data-ttu-id="bb1ad-158">Идентификатор пользователя или участника-службы, которая создана подписка.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="bb1ad-159">Если используется приложение делегированных разрешений на создание подписки, это поле содержит код вызова приложения от имени владельца пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="bb1ad-160">Если приложение разрешения приложения, это поле содержит идентификатор участника-службы, соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="bb1ad-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="bb1ad-162">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="bb1ad-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="bb1ad-163">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bb1ad-163">Resource</span></span>            | <span data-ttu-id="bb1ad-164">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="bb1ad-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="bb1ad-165">Почта</span><span class="sxs-lookup"><span data-stu-id="bb1ad-165">Mail</span></span>                | <span data-ttu-id="bb1ad-166">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bb1ad-167">Календарь</span><span class="sxs-lookup"><span data-stu-id="bb1ad-167">Calendar</span></span>            | <span data-ttu-id="bb1ad-168">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bb1ad-169">Контакты</span><span class="sxs-lookup"><span data-stu-id="bb1ad-169">Contacts</span></span>            | <span data-ttu-id="bb1ad-170">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bb1ad-171">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="bb1ad-171">Group conversations</span></span> | <span data-ttu-id="bb1ad-172">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bb1ad-173">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="bb1ad-173">Drive root items</span></span>    | <span data-ttu-id="bb1ad-174">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="bb1ad-175">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="bb1ad-175">Security alerts</span></span>     | <span data-ttu-id="bb1ad-176">43200 минут (в разделе 30 дней)</span><span class="sxs-lookup"><span data-stu-id="bb1ad-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="bb1ad-177">**Примечание:** Поддерживаемые значения не должна превышать существующих приложений и новых приложений.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="bb1ad-178">В дальнейшем все запросы, чтобы создать или обновить подписку за пределы максимальное значение завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="bb1ad-179">Связи</span><span class="sxs-lookup"><span data-stu-id="bb1ad-179">Relationships</span></span>

<span data-ttu-id="bb1ad-180">Нет</span><span class="sxs-lookup"><span data-stu-id="bb1ad-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="bb1ad-181">Методы</span><span class="sxs-lookup"><span data-stu-id="bb1ad-181">Methods</span></span>

| <span data-ttu-id="bb1ad-182">Метод</span><span class="sxs-lookup"><span data-stu-id="bb1ad-182">Method</span></span> | <span data-ttu-id="bb1ad-183">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb1ad-183">Return Type</span></span> | <span data-ttu-id="bb1ad-184">Описание</span><span class="sxs-lookup"><span data-stu-id="bb1ad-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="bb1ad-185">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="bb1ad-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="bb1ad-186">subscription</span><span class="sxs-lookup"><span data-stu-id="bb1ad-186">subscription</span></span>](subscription.md) | <span data-ttu-id="bb1ad-187">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="bb1ad-188">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="bb1ad-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="bb1ad-189">subscription</span><span class="sxs-lookup"><span data-stu-id="bb1ad-189">subscription</span></span>](subscription.md) | <span data-ttu-id="bb1ad-190">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="bb1ad-191">Список подписок</span><span class="sxs-lookup"><span data-stu-id="bb1ad-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="bb1ad-192">subscription</span><span class="sxs-lookup"><span data-stu-id="bb1ad-192">subscription</span></span>](subscription.md) | <span data-ttu-id="bb1ad-193">Список активных подписок.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="bb1ad-194">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="bb1ad-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="bb1ad-195">subscription</span><span class="sxs-lookup"><span data-stu-id="bb1ad-195">subscription</span></span>](subscription.md) | <span data-ttu-id="bb1ad-196">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="bb1ad-197">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="bb1ad-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="bb1ad-198">Нет</span><span class="sxs-lookup"><span data-stu-id="bb1ad-198">None</span></span> |<span data-ttu-id="bb1ad-199">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="bb1ad-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
