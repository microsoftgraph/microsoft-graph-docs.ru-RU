# <a name="create-single-value-extended-property"></a><span data-ttu-id="bd06f-101">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="bd06f-101">Create single-value extended property</span></span>

<span data-ttu-id="bd06f-102">Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd06f-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="bd06f-103">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="bd06f-103">The following user resources are supported:</span></span>

- <span data-ttu-id="bd06f-104">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="bd06f-104">[message](../resources/message.md)</span></span>
- <span data-ttu-id="bd06f-105">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="bd06f-105">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="bd06f-106">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="bd06f-106">[event](../resources/event.md)</span></span>
- <span data-ttu-id="bd06f-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="bd06f-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="bd06f-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="bd06f-108">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="bd06f-109">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-109">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="bd06f-110">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="bd06f-110">As well as the following group resources:</span></span>

- <span data-ttu-id="bd06f-111">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="bd06f-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="bd06f-112">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="bd06f-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="bd06f-113">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="bd06f-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="bd06f-114">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd06f-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd06f-115">Permissions</span></span>
<span data-ttu-id="bd06f-p101">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, в котором создается расширенное свойство). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="bd06f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd06f-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="bd06f-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd06f-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="bd06f-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd06f-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="bd06f-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd06f-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="bd06f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd06f-122">HTTP request</span></span>
<span data-ttu-id="bd06f-123">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd06f-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="bd06f-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="bd06f-127">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="bd06f-127">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="bd06f-128">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="bd06f-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="bd06f-129">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="bd06f-129">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```


## <a name="parameters"></a><span data-ttu-id="bd06f-130">Параметры</span><span class="sxs-lookup"><span data-stu-id="bd06f-130">Parameters</span></span>
|<span data-ttu-id="bd06f-131">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="bd06f-131">**Parameter**</span></span>|<span data-ttu-id="bd06f-132">**Тип**</span><span class="sxs-lookup"><span data-stu-id="bd06f-132">**Type**</span></span>|<span data-ttu-id="bd06f-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd06f-133">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bd06f-134">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="bd06f-134">_URL parameters_</span></span>|
|<span data-ttu-id="bd06f-135">id</span><span class="sxs-lookup"><span data-stu-id="bd06f-135">id</span></span>|<span data-ttu-id="bd06f-136">string</span><span class="sxs-lookup"><span data-stu-id="bd06f-136">string</span></span>|<span data-ttu-id="bd06f-p103">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p103">A unique identifier for an object in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="bd06f-139">_Параметры тела_</span><span class="sxs-lookup"><span data-stu-id="bd06f-139">_Body parameters_</span></span>|
|<span data-ttu-id="bd06f-140">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bd06f-140">singleValueExtendedProperties</span></span>|<span data-ttu-id="bd06f-141">Коллекция [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)</span><span class="sxs-lookup"><span data-stu-id="bd06f-141">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="bd06f-142">Массив из одного или нескольких расширенных свойств с одним значением.</span><span class="sxs-lookup"><span data-stu-id="bd06f-142">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="bd06f-143">id</span><span class="sxs-lookup"><span data-stu-id="bd06f-143">id</span></span>|<span data-ttu-id="bd06f-144">Строка</span><span class="sxs-lookup"><span data-stu-id="bd06f-144">String</span></span>|<span data-ttu-id="bd06f-p104">Чтобы идентифицировать свойства в коллекции **singleValueExtendedProperties**, для каждого из них укажите этот параметр. Свойство должно быть одного из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="bd06f-149">значение</span><span class="sxs-lookup"><span data-stu-id="bd06f-149">value</span></span>|<span data-ttu-id="bd06f-150">string</span><span class="sxs-lookup"><span data-stu-id="bd06f-150">string</span></span>|<span data-ttu-id="bd06f-p105">Для каждого свойства из коллекции **singleValueExtendedProperties** следует указать значение. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bd06f-153">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd06f-153">Request headers</span></span>
| <span data-ttu-id="bd06f-154">Имя</span><span class="sxs-lookup"><span data-stu-id="bd06f-154">Name</span></span>       | <span data-ttu-id="bd06f-155">Значение</span><span class="sxs-lookup"><span data-stu-id="bd06f-155">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bd06f-156">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd06f-156">Authorization</span></span> | <span data-ttu-id="bd06f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd06f-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd06f-159">Content-Type</span></span> | <span data-ttu-id="bd06f-160">application/json</span><span class="sxs-lookup"><span data-stu-id="bd06f-160">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd06f-161">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd06f-161">Request body</span></span>

<span data-ttu-id="bd06f-162">Предоставьте тело JSON каждого объекта [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) в свойстве коллекции **singleValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd06f-162">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

<span data-ttu-id="bd06f-163">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **singleValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd06f-163">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="bd06f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd06f-164">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="bd06f-165">Код отклика</span><span class="sxs-lookup"><span data-stu-id="bd06f-165">Response code</span></span>
<span data-ttu-id="bd06f-166">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="bd06f-166">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="bd06f-167">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="bd06f-167">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="bd06f-168">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="bd06f-168">Response body</span></span>

<span data-ttu-id="bd06f-p107">При создании расширенного свойства отклик будет включать только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы отобразить только что созданное расширенное свойство, [примените к экземпляру, содержащему это расширенное свойство, параметр $expand](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="bd06f-171">Когда вы создаете расширенное свойство в _новом_ экземпляре [group post](../resources/post.md) при ответе на беседу или публикацию, отклик будет включать только код отклика, но не новую публикацию или расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="bd06f-171">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="bd06f-172">Пример</span><span class="sxs-lookup"><span data-stu-id="bd06f-172">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="bd06f-173">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="bd06f-173">Request 1</span></span>

<span data-ttu-id="bd06f-p108">Первый пример показывает создание нового события и расширенного свойства с одним значением с помощью одной и той же операции POST. Помимо свойств, которые вы обычно указываете для нового события, тело запроса включает коллекцию **singleValueExtendedProperties**, которая содержит одно расширенное свойство с одним значением, и следующие данные для этого свойства:</span><span class="sxs-lookup"><span data-stu-id="bd06f-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="bd06f-176">**id** (указывает тип свойства как `String`), GUID и свойство `Fun`.</span><span class="sxs-lookup"><span data-stu-id="bd06f-176">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="bd06f-177">**value** (указывает `Food` как значение свойства `Fun`).</span><span class="sxs-lookup"><span data-stu-id="bd06f-177">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="bd06f-178">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="bd06f-178">Response 1</span></span>

<span data-ttu-id="bd06f-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user_post_events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="bd06f-181">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-181">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="bd06f-182">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="bd06f-182">Request 2</span></span>

<span data-ttu-id="bd06f-p110">Второй пример показывает создание расширенного свойства с одним значением для указанного существующего сообщения. Это расширенное свойство — единственный элемент в массиве **singleValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="bd06f-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="bd06f-186">**id** (указывает тип свойства как `String`), GUID и свойство `Color`.</span><span class="sxs-lookup"><span data-stu-id="bd06f-186">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="bd06f-187">**value** (указывает `Green` как значение свойства `Color`).</span><span class="sxs-lookup"><span data-stu-id="bd06f-187">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="bd06f-188">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="bd06f-188">Response 2</span></span>

<span data-ttu-id="bd06f-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message_update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="bd06f-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="bd06f-191">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="bd06f-191">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

