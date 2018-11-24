# <a name="subscription-resource-type"></a><span data-ttu-id="c452b-101">Тип ресурса подписки</span><span class="sxs-lookup"><span data-stu-id="c452b-101">subscription resource type</span></span>

<span data-ttu-id="c452b-102">Подписка позволяет клиентского приложения, чтобы получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c452b-102">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="c452b-103">На данный момент подписки включены следующие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="c452b-103">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="c452b-104">Почты, события и контакты из Outlook.</span><span class="sxs-lookup"><span data-stu-id="c452b-104">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="c452b-105">Беседы в группах Office.</span><span class="sxs-lookup"><span data-stu-id="c452b-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="c452b-106">Диск корневым элементов из службы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c452b-106">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="c452b-107">Пользователи и группы из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c452b-107">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="c452b-108">Оповещения о от безопасности Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="c452b-108">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c452b-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c452b-109">JSON representation</span></span>

<span data-ttu-id="c452b-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c452b-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c452b-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c452b-111">Properties</span></span>

| <span data-ttu-id="c452b-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c452b-112">Property</span></span> | <span data-ttu-id="c452b-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c452b-113">Type</span></span> | <span data-ttu-id="c452b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c452b-114">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c452b-115">changeType</span><span class="sxs-lookup"><span data-stu-id="c452b-115">changeType</span></span> | <span data-ttu-id="c452b-116">строка</span><span class="sxs-lookup"><span data-stu-id="c452b-116">string</span></span> | <span data-ttu-id="c452b-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c452b-117">Required.</span></span> <span data-ttu-id="c452b-118">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="c452b-118">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="c452b-119">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c452b-119">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="c452b-120">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="c452b-120">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="c452b-121">Примечание: Диск корневого элемента уведомлений поддерживает только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="c452b-121">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="c452b-122">Уведомления пользователей и групп поддержки `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="c452b-122">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="c452b-123">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="c452b-123">notificationUrl</span></span> | <span data-ttu-id="c452b-124">строка</span><span class="sxs-lookup"><span data-stu-id="c452b-124">string</span></span> | <span data-ttu-id="c452b-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c452b-125">Required.</span></span> <span data-ttu-id="c452b-126">URL-адрес конечной точки, который будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="c452b-126">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="c452b-127">Этот URL-адрес необходимо использовать протокол HTTPS протокола.</span><span class="sxs-lookup"><span data-stu-id="c452b-127">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="c452b-128">resource</span><span class="sxs-lookup"><span data-stu-id="c452b-128">resource</span></span> | <span data-ttu-id="c452b-129">строка</span><span class="sxs-lookup"><span data-stu-id="c452b-129">string</span></span> | <span data-ttu-id="c452b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c452b-130">Required.</span></span> <span data-ttu-id="c452b-131">Указывает ресурс, к которому будет выполняться мониторинг изменений.</span><span class="sxs-lookup"><span data-stu-id="c452b-131">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="c452b-132">Не включать базовый URL-адрес (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="c452b-132">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="c452b-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c452b-133">expirationDateTime</span></span> | [<span data-ttu-id="c452b-134">dateTime</span><span class="sxs-lookup"><span data-stu-id="c452b-134">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="c452b-135">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="c452b-135">Required.</span></span> <span data-ttu-id="c452b-136">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="c452b-136">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="c452b-137">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="c452b-137">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="c452b-138">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="c452b-138">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="c452b-139">clientState</span><span class="sxs-lookup"><span data-stu-id="c452b-139">clientState</span></span> | <span data-ttu-id="c452b-140">строка</span><span class="sxs-lookup"><span data-stu-id="c452b-140">string</span></span> | <span data-ttu-id="c452b-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c452b-141">Optional.</span></span> <span data-ttu-id="c452b-142">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="c452b-142">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="c452b-143">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="c452b-143">The maximum length is 128 characters.</span></span> <span data-ttu-id="c452b-144">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="c452b-144">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="c452b-145">id</span><span class="sxs-lookup"><span data-stu-id="c452b-145">id</span></span> | <span data-ttu-id="c452b-146">строка</span><span class="sxs-lookup"><span data-stu-id="c452b-146">string</span></span> | <span data-ttu-id="c452b-p108">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c452b-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="c452b-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="c452b-149">applicationId</span></span> | <span data-ttu-id="c452b-150">string</span><span class="sxs-lookup"><span data-stu-id="c452b-150">string</span></span> | <span data-ttu-id="c452b-151">Идентификатор приложения, используемого для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="c452b-151">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="c452b-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c452b-152">Read-only.</span></span> |
| <span data-ttu-id="c452b-153">creatorId</span><span class="sxs-lookup"><span data-stu-id="c452b-153">creatorId</span></span> | <span data-ttu-id="c452b-154">string</span><span class="sxs-lookup"><span data-stu-id="c452b-154">string</span></span> | <span data-ttu-id="c452b-155">Идентификатор пользователя или участника-службы, которая создана подписка.</span><span class="sxs-lookup"><span data-stu-id="c452b-155">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="c452b-156">Если используется приложение делегированных разрешений на создание подписки, это поле содержит код вызова приложения от имени владельца пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="c452b-156">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="c452b-157">Если приложение разрешения приложения, это поле содержит идентификатор участника-службы, соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="c452b-157">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="c452b-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c452b-158">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="c452b-159">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="c452b-159">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="c452b-160">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c452b-160">Resource</span></span>            | <span data-ttu-id="c452b-161">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="c452b-161">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="c452b-162">Почта</span><span class="sxs-lookup"><span data-stu-id="c452b-162">Mail</span></span>                | <span data-ttu-id="c452b-163">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="c452b-163">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c452b-164">Календарь</span><span class="sxs-lookup"><span data-stu-id="c452b-164">Calendar</span></span>            | <span data-ttu-id="c452b-165">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="c452b-165">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c452b-166">Контакты</span><span class="sxs-lookup"><span data-stu-id="c452b-166">Contacts</span></span>            | <span data-ttu-id="c452b-167">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="c452b-167">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c452b-168">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="c452b-168">Group conversations</span></span> | <span data-ttu-id="c452b-169">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="c452b-169">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c452b-170">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="c452b-170">Drive root items</span></span>    | <span data-ttu-id="c452b-171">4230 минут (в разделе 3 дня)</span><span class="sxs-lookup"><span data-stu-id="c452b-171">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c452b-172">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="c452b-172">Security alerts</span></span>     | <span data-ttu-id="c452b-173">43200 минут (в разделе 30 дней)</span><span class="sxs-lookup"><span data-stu-id="c452b-173">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="c452b-174">**Примечание:** Поддерживаемые значения не должна превышать существующих приложений и новых приложений.</span><span class="sxs-lookup"><span data-stu-id="c452b-174">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="c452b-175">В дальнейшем все запросы, чтобы создать или обновить подписку за пределы максимальное значение завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="c452b-175">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="c452b-176">Связи</span><span class="sxs-lookup"><span data-stu-id="c452b-176">Relationships</span></span>

<span data-ttu-id="c452b-177">Нет</span><span class="sxs-lookup"><span data-stu-id="c452b-177">None</span></span>

## <a name="methods"></a><span data-ttu-id="c452b-178">Методы</span><span class="sxs-lookup"><span data-stu-id="c452b-178">Methods</span></span>

| <span data-ttu-id="c452b-179">Метод</span><span class="sxs-lookup"><span data-stu-id="c452b-179">Method</span></span> | <span data-ttu-id="c452b-180">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c452b-180">Return Type</span></span> | <span data-ttu-id="c452b-181">Описание</span><span class="sxs-lookup"><span data-stu-id="c452b-181">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="c452b-182">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="c452b-182">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="c452b-183">subscription</span><span class="sxs-lookup"><span data-stu-id="c452b-183">subscription</span></span>](subscription.md) | <span data-ttu-id="c452b-184">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c452b-184">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="c452b-185">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="c452b-185">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="c452b-186">subscription</span><span class="sxs-lookup"><span data-stu-id="c452b-186">subscription</span></span>](subscription.md) | <span data-ttu-id="c452b-187">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="c452b-187">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="c452b-188">Список подписок</span><span class="sxs-lookup"><span data-stu-id="c452b-188">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="c452b-189">subscription</span><span class="sxs-lookup"><span data-stu-id="c452b-189">subscription</span></span>](subscription.md) | <span data-ttu-id="c452b-190">Список активных подписок.</span><span class="sxs-lookup"><span data-stu-id="c452b-190">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="c452b-191">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="c452b-191">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="c452b-192">subscription</span><span class="sxs-lookup"><span data-stu-id="c452b-192">subscription</span></span>](subscription.md) | <span data-ttu-id="c452b-193">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="c452b-193">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="c452b-194">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="c452b-194">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="c452b-195">Нет</span><span class="sxs-lookup"><span data-stu-id="c452b-195">None</span></span> |<span data-ttu-id="c452b-196">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="c452b-196">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
