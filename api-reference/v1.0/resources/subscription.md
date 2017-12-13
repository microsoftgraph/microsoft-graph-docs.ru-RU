# <a name="subscription-resource-type"></a><span data-ttu-id="d23a3-101">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="d23a3-101">Subscription Resource Type</span></span>
<span data-ttu-id="d23a3-102">Подписка позволяет клиентскому приложению получать уведомления о данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d23a3-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph. Currently subscriptions are enabled for the following datasets:</span></span> <span data-ttu-id="d23a3-103">На данный момент подписки включены для указанных ниже наборов данных.</span><span class="sxs-lookup"><span data-stu-id="d23a3-103">Currently, subscriptions are enabled for the following datasets:</span></span>

1. <span data-ttu-id="d23a3-104">Почта, события и контакты из Outlook.</span><span class="sxs-lookup"><span data-stu-id="d23a3-104">Mail, events, and contacts from Outlook</span></span>
1. <span data-ttu-id="d23a3-105">Беседы в группах Office.</span><span class="sxs-lookup"><span data-stu-id="d23a3-105">Conversations from Office Groups.</span></span>
1. <span data-ttu-id="d23a3-106">Корневые элементы диска в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d23a3-106">Drive root items from OneDrive</span></span> 


## <a name="json-representation"></a><span data-ttu-id="d23a3-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d23a3-107">JSON representation</span></span>

<span data-ttu-id="d23a3-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d23a3-108">Here is a JSON representation of the resource.</span></span>

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
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d23a3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d23a3-109">Properties</span></span>
| <span data-ttu-id="d23a3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d23a3-110">Property</span></span>     | <span data-ttu-id="d23a3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d23a3-111">Type</span></span>   |<span data-ttu-id="d23a3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d23a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d23a3-113">changeType</span><span class="sxs-lookup"><span data-stu-id="d23a3-113">changeType</span></span>|<span data-ttu-id="d23a3-114">string</span><span class="sxs-lookup"><span data-stu-id="d23a3-114">string</span></span>|<span data-ttu-id="d23a3-115">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="d23a3-115">Indicates the type of change in the subscribed resource that will raise a notification. The supported values are: , , . Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="d23a3-116">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d23a3-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="d23a3-117">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="d23a3-117">Multiple values can be combined using a comma-separated list.</span></span>|
|<span data-ttu-id="d23a3-118">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="d23a3-118">notificationUrl</span></span>|<span data-ttu-id="d23a3-119">string</span><span class="sxs-lookup"><span data-stu-id="d23a3-119">string</span></span>|<span data-ttu-id="d23a3-p103">URL-адрес конечной точки, которая будет получать уведомления. Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="d23a3-p103">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span>|
|<span data-ttu-id="d23a3-122">ресурс</span><span class="sxs-lookup"><span data-stu-id="d23a3-122">resource</span></span>|<span data-ttu-id="d23a3-123">string</span><span class="sxs-lookup"><span data-stu-id="d23a3-123">string</span></span>|<span data-ttu-id="d23a3-p104">Указывает ресурс, для которого будут отслеживаться изменения. Не включайте базовый URL-адрес (https://graph.microsoft.com/v1.0/).</span><span class="sxs-lookup"><span data-stu-id="d23a3-p104">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span>|
|<span data-ttu-id="d23a3-126">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d23a3-126">expirationDateTime</span></span>|[<span data-ttu-id="d23a3-127">dateTime</span><span class="sxs-lookup"><span data-stu-id="d23a3-127">dateTime</span></span>](http://tools.ietf.org/html/rfc3339)|<span data-ttu-id="d23a3-128">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="d23a3-128">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="d23a3-129">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="d23a3-129">Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum values.</span></span>  <span data-ttu-id="d23a3-130">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="d23a3-130">See the table below for maximum supported subscription length of time.</span></span> |
|<span data-ttu-id="d23a3-131">clientState</span><span class="sxs-lookup"><span data-stu-id="d23a3-131">clientState</span></span>|<span data-ttu-id="d23a3-132">string</span><span class="sxs-lookup"><span data-stu-id="d23a3-132">string</span></span>|<span data-ttu-id="d23a3-133">Указывает значение свойства `clientState`, отправляемого службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="d23a3-133">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="d23a3-134">Максимальная длина составляет 128 символов.</span><span class="sxs-lookup"><span data-stu-id="d23a3-134">The maximum length is 255 characters.</span></span> <span data-ttu-id="d23a3-135">Клиент может проверить, пришло ли уведомление от службы, сравнив значение свойства `clientState`, отправленного с подпиской, со значением свойства `clientState`, получаемого с каждым уведомлением.</span><span class="sxs-lookup"><span data-stu-id="d23a3-135">Specifies the value of the  property sent by the service in each notification. The maximum length is 128 characters. The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span>|
|<span data-ttu-id="d23a3-136">id</span><span class="sxs-lookup"><span data-stu-id="d23a3-136">id</span></span>|<span data-ttu-id="d23a3-137">string</span><span class="sxs-lookup"><span data-stu-id="d23a3-137">string</span></span>|<span data-ttu-id="d23a3-p107">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23a3-p107">Unique identifier for the subscription. Read-only.</span></span>|

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="d23a3-140">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="d23a3-140">Maximum length of subscription per resource type</span></span>
| <span data-ttu-id="d23a3-141">Ресурс</span><span class="sxs-lookup"><span data-stu-id="d23a3-141">Resource</span></span> | <span data-ttu-id="d23a3-142">Максимальный срок действия</span><span class="sxs-lookup"><span data-stu-id="d23a3-142">Maximum Expiration Time</span></span> |
|:---------------------|:--------------------|
|<span data-ttu-id="d23a3-143">Почта</span><span class="sxs-lookup"><span data-stu-id="d23a3-143">Mail</span></span>| <span data-ttu-id="d23a3-144">4230 минут.</span><span class="sxs-lookup"><span data-stu-id="d23a3-144">4230 minutes.</span></span>|
|<span data-ttu-id="d23a3-145">Календарь</span><span class="sxs-lookup"><span data-stu-id="d23a3-145">Calendar</span></span>| <span data-ttu-id="d23a3-146">4230 минут.</span><span class="sxs-lookup"><span data-stu-id="d23a3-146">4230 minutes.</span></span>|
|<span data-ttu-id="d23a3-147">Контакты</span><span class="sxs-lookup"><span data-stu-id="d23a3-147">Contacts</span></span>| <span data-ttu-id="d23a3-148">4230 минут.</span><span class="sxs-lookup"><span data-stu-id="d23a3-148">4230 minutes.</span></span>|
|<span data-ttu-id="d23a3-149">Беседы группы</span><span class="sxs-lookup"><span data-stu-id="d23a3-149">Group conversations</span></span>| <span data-ttu-id="d23a3-150">4230 минут.</span><span class="sxs-lookup"><span data-stu-id="d23a3-150">4230 minutes.</span></span>|
|<span data-ttu-id="d23a3-151">Элементы в корне диска</span><span class="sxs-lookup"><span data-stu-id="d23a3-151">Drive root items</span></span>| <span data-ttu-id="d23a3-152">43 200 минут.</span><span class="sxs-lookup"><span data-stu-id="d23a3-152">43200 minutes.</span></span> <span data-ttu-id="d23a3-153">Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="d23a3-153">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="d23a3-154">В будущих выпусках значения, которые больше, не будут разрешены.</span><span class="sxs-lookup"><span data-stu-id="d23a3-154">Higher values won't be permitted in upcoming releases.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d23a3-155">Связи</span><span class="sxs-lookup"><span data-stu-id="d23a3-155">Relationships</span></span>
<span data-ttu-id="d23a3-156">Нет</span><span class="sxs-lookup"><span data-stu-id="d23a3-156">None</span></span>


## <a name="methods"></a><span data-ttu-id="d23a3-157">Методы</span><span class="sxs-lookup"><span data-stu-id="d23a3-157">Methods</span></span>

| <span data-ttu-id="d23a3-158">Метод</span><span class="sxs-lookup"><span data-stu-id="d23a3-158">Method</span></span>           | <span data-ttu-id="d23a3-159">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d23a3-159">Return Type</span></span>    |<span data-ttu-id="d23a3-160">Описание</span><span class="sxs-lookup"><span data-stu-id="d23a3-160">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d23a3-161">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="d23a3-161">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="d23a3-162">subscription</span><span class="sxs-lookup"><span data-stu-id="d23a3-162">subscription</span></span>](subscription.md) |<span data-ttu-id="d23a3-163">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d23a3-163">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span>|
|[<span data-ttu-id="d23a3-164">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="d23a3-164">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="d23a3-165">subscription</span><span class="sxs-lookup"><span data-stu-id="d23a3-165">subscription</span></span>](subscription.md) |<span data-ttu-id="d23a3-166">Обновление подписки путем изменения ее срока действия.</span><span class="sxs-lookup"><span data-stu-id="d23a3-166">Renews a subscription by updating its expiration time.</span></span>|
|[<span data-ttu-id="d23a3-167">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="d23a3-167">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="d23a3-168">subscription</span><span class="sxs-lookup"><span data-stu-id="d23a3-168">subscription</span></span>](subscription.md) |<span data-ttu-id="d23a3-169">Чтение свойств и связей объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="d23a3-169">Reads properties and relationships of subscription object.</span></span>|
|[<span data-ttu-id="d23a3-170">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="d23a3-170">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="d23a3-171">Нет</span><span class="sxs-lookup"><span data-stu-id="d23a3-171">None</span></span> |<span data-ttu-id="d23a3-172">Удаление объекта subscription.</span><span class="sxs-lookup"><span data-stu-id="d23a3-172">Deletes a subscription object.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
