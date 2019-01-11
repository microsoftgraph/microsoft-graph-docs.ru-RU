---
title: Тип ресурса подписки
description: 'Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены следующие ресурсы:'
localization_priority: Priority
ms.openlocfilehash: b70daca8eb0f7c303173945b3cacf2cf53af56ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867013"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="1e7f0-104">Тип ресурса подписки</span><span class="sxs-lookup"><span data-stu-id="1e7f0-104">subscription resource type</span></span>

<span data-ttu-id="1e7f0-105">Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="1e7f0-106">На данный момент подписки включены следующие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="1e7f0-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="1e7f0-107">Почты, события и контакты из Outlook.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="1e7f0-108">Беседы в группах Office.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="1e7f0-109">Диск корневым элементов из службы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="1e7f0-110">Пользователи и группы из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="1e7f0-111">Оповещения о от безопасности Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e7f0-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e7f0-112">JSON representation</span></span>

<span data-ttu-id="1e7f0-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e7f0-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e7f0-114">Properties</span></span>

| <span data-ttu-id="1e7f0-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e7f0-115">Property</span></span> | <span data-ttu-id="1e7f0-116">Тип</span><span class="sxs-lookup"><span data-stu-id="1e7f0-116">Type</span></span> | <span data-ttu-id="1e7f0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1e7f0-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1e7f0-118">changeType</span><span class="sxs-lookup"><span data-stu-id="1e7f0-118">changeType</span></span> | <span data-ttu-id="1e7f0-119">строка</span><span class="sxs-lookup"><span data-stu-id="1e7f0-119">string</span></span> | <span data-ttu-id="1e7f0-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-120">Required.</span></span> <span data-ttu-id="1e7f0-121">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="1e7f0-122">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="1e7f0-123">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="1e7f0-124">Примечание: Диск корневого элемента уведомлений поддерживает только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="1e7f0-125">Уведомления пользователей и групп поддержки `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="1e7f0-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="1e7f0-126">notificationUrl</span></span> | <span data-ttu-id="1e7f0-127">строка</span><span class="sxs-lookup"><span data-stu-id="1e7f0-127">string</span></span> | <span data-ttu-id="1e7f0-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-128">Required.</span></span> <span data-ttu-id="1e7f0-129">URL-адрес конечной точки, который будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="1e7f0-130">Этот URL-адрес необходимо использовать протокол HTTPS протокола.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="1e7f0-131">resource</span><span class="sxs-lookup"><span data-stu-id="1e7f0-131">resource</span></span> | <span data-ttu-id="1e7f0-132">строка</span><span class="sxs-lookup"><span data-stu-id="1e7f0-132">string</span></span> | <span data-ttu-id="1e7f0-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-133">Required.</span></span> <span data-ttu-id="1e7f0-134">Указывает ресурс, к которому будет выполняться мониторинг изменений.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1e7f0-135">Не включать базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="1e7f0-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="1e7f0-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e7f0-136">expirationDateTime</span></span> | [<span data-ttu-id="1e7f0-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="1e7f0-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="1e7f0-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-138">Required.</span></span> <span data-ttu-id="1e7f0-139">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="1e7f0-140">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="1e7f0-141">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="1e7f0-142">clientState</span><span class="sxs-lookup"><span data-stu-id="1e7f0-142">clientState</span></span> | <span data-ttu-id="1e7f0-143">строка</span><span class="sxs-lookup"><span data-stu-id="1e7f0-143">string</span></span> | <span data-ttu-id="1e7f0-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-144">Optional.</span></span> <span data-ttu-id="1e7f0-145">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="1e7f0-146">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="1e7f0-147">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="1e7f0-148">id</span><span class="sxs-lookup"><span data-stu-id="1e7f0-148">id</span></span> | <span data-ttu-id="1e7f0-149">строка</span><span class="sxs-lookup"><span data-stu-id="1e7f0-149">string</span></span> | <span data-ttu-id="1e7f0-p109">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="1e7f0-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="1e7f0-152">applicationId</span></span> | <span data-ttu-id="1e7f0-153">string</span><span class="sxs-lookup"><span data-stu-id="1e7f0-153">string</span></span> | <span data-ttu-id="1e7f0-154">Идентификатор приложения, используемого для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="1e7f0-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-155">Read-only.</span></span> |
| <span data-ttu-id="1e7f0-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="1e7f0-156">creatorId</span></span> | <span data-ttu-id="1e7f0-157">string</span><span class="sxs-lookup"><span data-stu-id="1e7f0-157">string</span></span> | <span data-ttu-id="1e7f0-158">Идентификатор пользователя или участника-службы, которая создана подписка.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="1e7f0-159">Если используется приложение делегированных разрешений на создание подписки, это поле содержит код вызова приложения от имени владельца пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="1e7f0-160">Если приложение разрешения приложения, это поле содержит идентификатор участника-службы, соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="1e7f0-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="1e7f0-162">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="1e7f0-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="1e7f0-163">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1e7f0-163">Resource</span></span>            | <span data-ttu-id="1e7f0-164">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="1e7f0-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="1e7f0-165">Почта</span><span class="sxs-lookup"><span data-stu-id="1e7f0-165">Mail</span></span>                | <span data-ttu-id="1e7f0-166">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e7f0-167">Календарь</span><span class="sxs-lookup"><span data-stu-id="1e7f0-167">Calendar</span></span>            | <span data-ttu-id="1e7f0-168">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e7f0-169">Контакты</span><span class="sxs-lookup"><span data-stu-id="1e7f0-169">Contacts</span></span>            | <span data-ttu-id="1e7f0-170">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e7f0-171">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="1e7f0-171">Group conversations</span></span> | <span data-ttu-id="1e7f0-172">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e7f0-173">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="1e7f0-173">Drive root items</span></span>    | <span data-ttu-id="1e7f0-174">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e7f0-175">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="1e7f0-175">Security alerts</span></span>     | <span data-ttu-id="1e7f0-176">43200 минут (в разделе 30 дней)</span><span class="sxs-lookup"><span data-stu-id="1e7f0-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="1e7f0-177">**Примечание:** Поддерживаемые значения не должна превышать существующих приложений и новых приложений.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="1e7f0-178">В дальнейшем все запросы, чтобы создать или обновить подписку за пределы максимальное значение завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="1e7f0-179">Связи</span><span class="sxs-lookup"><span data-stu-id="1e7f0-179">Relationships</span></span>

<span data-ttu-id="1e7f0-180">Нет</span><span class="sxs-lookup"><span data-stu-id="1e7f0-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="1e7f0-181">Методы</span><span class="sxs-lookup"><span data-stu-id="1e7f0-181">Methods</span></span>

| <span data-ttu-id="1e7f0-182">Метод</span><span class="sxs-lookup"><span data-stu-id="1e7f0-182">Method</span></span> | <span data-ttu-id="1e7f0-183">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e7f0-183">Return Type</span></span> | <span data-ttu-id="1e7f0-184">Описание</span><span class="sxs-lookup"><span data-stu-id="1e7f0-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="1e7f0-185">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1e7f0-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="1e7f0-186">subscription</span><span class="sxs-lookup"><span data-stu-id="1e7f0-186">subscription</span></span>](subscription.md) | <span data-ttu-id="1e7f0-187">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="1e7f0-188">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="1e7f0-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="1e7f0-189">subscription</span><span class="sxs-lookup"><span data-stu-id="1e7f0-189">subscription</span></span>](subscription.md) | <span data-ttu-id="1e7f0-190">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="1e7f0-191">Список подписок</span><span class="sxs-lookup"><span data-stu-id="1e7f0-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="1e7f0-192">subscription</span><span class="sxs-lookup"><span data-stu-id="1e7f0-192">subscription</span></span>](subscription.md) | <span data-ttu-id="1e7f0-193">Список активных подписок.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="1e7f0-194">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="1e7f0-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="1e7f0-195">subscription</span><span class="sxs-lookup"><span data-stu-id="1e7f0-195">subscription</span></span>](subscription.md) | <span data-ttu-id="1e7f0-196">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="1e7f0-197">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="1e7f0-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="1e7f0-198">Нет</span><span class="sxs-lookup"><span data-stu-id="1e7f0-198">None</span></span> |<span data-ttu-id="1e7f0-199">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="1e7f0-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
