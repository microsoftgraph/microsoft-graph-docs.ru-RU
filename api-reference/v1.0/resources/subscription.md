# <a name="subscription-resource-type"></a><span data-ttu-id="4002e-101">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="4002e-101">Subscription resource type</span></span>

<span data-ttu-id="4002e-102">Подписка позволяет клиентскому приложению получать уведомления о данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4002e-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="4002e-103">На данный момент, в подписки включены следующие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="4002e-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="4002e-104">Почта, события и контакты из Outlook.</span><span class="sxs-lookup"><span data-stu-id="4002e-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="4002e-105">Беседы в группах Office</span><span class="sxs-lookup"><span data-stu-id="4002e-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="4002e-106">Корневые элементы диска в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4002e-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="4002e-107">Пользователи и группы из Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4002e-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="4002e-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4002e-108">JSON representation</span></span>

<span data-ttu-id="4002e-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4002e-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4002e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4002e-110">Properties</span></span>

| <span data-ttu-id="4002e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="4002e-111">Property</span></span> | <span data-ttu-id="4002e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4002e-112">Type</span></span> | <span data-ttu-id="4002e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4002e-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4002e-114">changeType</span><span class="sxs-lookup"><span data-stu-id="4002e-114">changeType</span></span> | <span data-ttu-id="4002e-115">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-115">string</span></span> | <span data-ttu-id="4002e-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4002e-116">Required.</span></span> <span data-ttu-id="4002e-117">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="4002e-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="4002e-118">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="4002e-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="4002e-119">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="4002e-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="4002e-120">Примечание: Диск корневого элемента уведомлений поддерживает только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="4002e-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="4002e-121">Уведомления пользователей и групп поддержки `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="4002e-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="4002e-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="4002e-122">notificationUrl</span></span> | <span data-ttu-id="4002e-123">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-123">string</span></span> | <span data-ttu-id="4002e-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4002e-124">Required.</span></span> <span data-ttu-id="4002e-125">URL-адрес конечной точки, который будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="4002e-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="4002e-126">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4002e-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="4002e-127">resource</span><span class="sxs-lookup"><span data-stu-id="4002e-127">resource</span></span> | <span data-ttu-id="4002e-128">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-128">string</span></span> | <span data-ttu-id="4002e-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4002e-129">Required.</span></span> <span data-ttu-id="4002e-130">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="4002e-130">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span> <span data-ttu-id="4002e-131">Не включает базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="4002e-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="4002e-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4002e-132">expirationDateTime</span></span> | [<span data-ttu-id="4002e-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="4002e-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="4002e-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4002e-134">Required.</span></span> <span data-ttu-id="4002e-135">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="4002e-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="4002e-136">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="4002e-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="4002e-137">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="4002e-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="4002e-138">clientState</span><span class="sxs-lookup"><span data-stu-id="4002e-138">clientState</span></span> | <span data-ttu-id="4002e-139">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-139">string</span></span> | <span data-ttu-id="4002e-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4002e-140">Optional.</span></span> <span data-ttu-id="4002e-141">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="4002e-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="4002e-142">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="4002e-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="4002e-143">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="4002e-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="4002e-144">id</span><span class="sxs-lookup"><span data-stu-id="4002e-144">id</span></span> | <span data-ttu-id="4002e-145">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-145">string</span></span> | <span data-ttu-id="4002e-p108">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4002e-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="4002e-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="4002e-148">applicationId</span></span> | <span data-ttu-id="4002e-149">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-149">string</span></span> | <span data-ttu-id="4002e-150">Идентификатор приложения, используемого для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="4002e-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="4002e-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4002e-151">Read-only.</span></span> |
| <span data-ttu-id="4002e-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="4002e-152">creatorId</span></span> | <span data-ttu-id="4002e-153">строка</span><span class="sxs-lookup"><span data-stu-id="4002e-153">string</span></span> | <span data-ttu-id="4002e-154">Идентификатор пользователя или субъекта-службы, который создал подписку.</span><span class="sxs-lookup"><span data-stu-id="4002e-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="4002e-155">Если используется приложение делегированных разрешений на создание подписки, это поле содержит код вызова приложения от имени пользователя, выполнившего вход в приложение.</span><span class="sxs-lookup"><span data-stu-id="4002e-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="4002e-156">Если приложение использовало разрешения приложения, это поле содержит идентификатор субъекта-службы соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4002e-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="4002e-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4002e-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="4002e-158">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="4002e-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="4002e-159">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4002e-159">Resource</span></span>            | <span data-ttu-id="4002e-160">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="4002e-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="4002e-161">Почта</span><span class="sxs-lookup"><span data-stu-id="4002e-161">Mail</span></span>                | <span data-ttu-id="4002e-162">4320 минут (3 дня)</span><span class="sxs-lookup"><span data-stu-id="4002e-162">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="4002e-163">Календарь</span><span class="sxs-lookup"><span data-stu-id="4002e-163">Calendar</span></span>            | <span data-ttu-id="4002e-164">4320 минут (3 дня)</span><span class="sxs-lookup"><span data-stu-id="4002e-164">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="4002e-165">Контакты</span><span class="sxs-lookup"><span data-stu-id="4002e-165">Contacts</span></span>            | <span data-ttu-id="4002e-166">4320 минут (3 дня)</span><span class="sxs-lookup"><span data-stu-id="4002e-166">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="4002e-167">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="4002e-167">Group conversations</span></span> | <span data-ttu-id="4002e-168">4320 минут (3 дня)</span><span class="sxs-lookup"><span data-stu-id="4002e-168">4320 minutes (3 days)</span></span>    |
| <span data-ttu-id="4002e-169">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="4002e-169">Drive root items</span></span>    | <span data-ttu-id="4002e-170">4320 минут (3 дня)</span><span class="sxs-lookup"><span data-stu-id="4002e-170">4320 minutes (3 days)</span></span> |

> <span data-ttu-id="4002e-171">** Примечание:**  Для существующих приложений и новых приложений не должно превышаться поддерживаемое значение.</span><span class="sxs-lookup"><span data-stu-id="4002e-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="4002e-172">В дальнейшем все запросы на создание или обновление подписки за пределами максимального значения завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4002e-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="4002e-173">Связи</span><span class="sxs-lookup"><span data-stu-id="4002e-173">Relationships</span></span>

<span data-ttu-id="4002e-174">Нет</span><span class="sxs-lookup"><span data-stu-id="4002e-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="4002e-175">Методы</span><span class="sxs-lookup"><span data-stu-id="4002e-175">Methods</span></span>

| <span data-ttu-id="4002e-176">Метод</span><span class="sxs-lookup"><span data-stu-id="4002e-176">Method</span></span> | <span data-ttu-id="4002e-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4002e-177">Return Type</span></span> | <span data-ttu-id="4002e-178">Описание</span><span class="sxs-lookup"><span data-stu-id="4002e-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="4002e-179">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="4002e-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="4002e-180">subscription</span><span class="sxs-lookup"><span data-stu-id="4002e-180">subscription</span></span>](subscription.md) | <span data-ttu-id="4002e-181">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4002e-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="4002e-182">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="4002e-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="4002e-183">subscription</span><span class="sxs-lookup"><span data-stu-id="4002e-183">subscription</span></span>](subscription.md) | <span data-ttu-id="4002e-184">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="4002e-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="4002e-185">Перечислить подписки</span><span class="sxs-lookup"><span data-stu-id="4002e-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="4002e-186">subscription</span><span class="sxs-lookup"><span data-stu-id="4002e-186">subscription</span></span>](subscription.md) | <span data-ttu-id="4002e-187">Список активных подписок.</span><span class="sxs-lookup"><span data-stu-id="4002e-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="4002e-188">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="4002e-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="4002e-189">subscription</span><span class="sxs-lookup"><span data-stu-id="4002e-189">subscription</span></span>](subscription.md) | <span data-ttu-id="4002e-190">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="4002e-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="4002e-191">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="4002e-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="4002e-192">Нет</span><span class="sxs-lookup"><span data-stu-id="4002e-192">None</span></span> |<span data-ttu-id="4002e-193">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="4002e-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
