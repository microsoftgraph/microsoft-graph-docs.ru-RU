# <a name="create-multi-value-extended-property"></a><span data-ttu-id="679eb-101">Создание многозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="679eb-101">Create multi-value extended property</span></span>

<span data-ttu-id="679eb-102">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="679eb-102">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="679eb-103">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="679eb-103">The following user resources are supported:</span></span>

- <span data-ttu-id="679eb-104">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="679eb-104">[message](../resources/message.md)</span></span>
- <span data-ttu-id="679eb-105">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="679eb-105">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="679eb-106">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="679eb-106">[event](../resources/event.md)</span></span>
- <span data-ttu-id="679eb-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="679eb-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="679eb-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="679eb-108">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="679eb-109">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-109">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="679eb-110">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="679eb-110">As well as the following group resources:</span></span>

- <span data-ttu-id="679eb-111">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="679eb-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="679eb-112">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="679eb-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="679eb-113">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="679eb-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="679eb-114">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="679eb-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="679eb-115">Permissions</span></span>
<span data-ttu-id="679eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, в котором создается расширенное свойство). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="679eb-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="679eb-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="679eb-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="679eb-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="679eb-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="679eb-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="679eb-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679eb-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="679eb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="679eb-122">HTTP request</span></span>
<span data-ttu-id="679eb-123">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="679eb-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="679eb-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="679eb-127">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="679eb-127">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="679eb-128">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="679eb-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="679eb-129">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="679eb-129">**Note** You cannot create an extended property in an existing group post.</span></span>

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


## <a name="parameters"></a><span data-ttu-id="679eb-130">Параметры</span><span class="sxs-lookup"><span data-stu-id="679eb-130">Parameters</span></span>
|<span data-ttu-id="679eb-131">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="679eb-131">**Parameter**</span></span>|<span data-ttu-id="679eb-132">**Тип**</span><span class="sxs-lookup"><span data-stu-id="679eb-132">**Type**</span></span>|<span data-ttu-id="679eb-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="679eb-133">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="679eb-134">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="679eb-134">_URL parameters_</span></span>|
|<span data-ttu-id="679eb-135">id</span><span class="sxs-lookup"><span data-stu-id="679eb-135">id</span></span>|<span data-ttu-id="679eb-136">string</span><span class="sxs-lookup"><span data-stu-id="679eb-136">string</span></span>|<span data-ttu-id="679eb-p103">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="679eb-p103">A unique identifier for an object in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="679eb-139">_Параметры тела_</span><span class="sxs-lookup"><span data-stu-id="679eb-139">_Body parameters_</span></span>|
|<span data-ttu-id="679eb-140">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="679eb-140">multiValueExtendedProperties</span></span>|<span data-ttu-id="679eb-141">Коллекция [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)</span><span class="sxs-lookup"><span data-stu-id="679eb-141">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="679eb-142">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="679eb-142">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="679eb-143">id</span><span class="sxs-lookup"><span data-stu-id="679eb-143">id</span></span>|<span data-ttu-id="679eb-144">Строка</span><span class="sxs-lookup"><span data-stu-id="679eb-144">String</span></span>|<span data-ttu-id="679eb-p104">Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="679eb-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="679eb-149">значение</span><span class="sxs-lookup"><span data-stu-id="679eb-149">value</span></span>|<span data-ttu-id="679eb-150">string</span><span class="sxs-lookup"><span data-stu-id="679eb-150">string</span></span>|<span data-ttu-id="679eb-p105">Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="679eb-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="679eb-153">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="679eb-153">Request headers</span></span>
| <span data-ttu-id="679eb-154">Имя</span><span class="sxs-lookup"><span data-stu-id="679eb-154">Name</span></span>       | <span data-ttu-id="679eb-155">Значение</span><span class="sxs-lookup"><span data-stu-id="679eb-155">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="679eb-156">Авторизация</span><span class="sxs-lookup"><span data-stu-id="679eb-156">Authorization</span></span> | <span data-ttu-id="679eb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="679eb-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="679eb-159">Content-Type</span><span class="sxs-lookup"><span data-stu-id="679eb-159">Content-Type</span></span> | <span data-ttu-id="679eb-160">application/json</span><span class="sxs-lookup"><span data-stu-id="679eb-160">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="679eb-161">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="679eb-161">Request body</span></span>

<span data-ttu-id="679eb-162">Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="679eb-162">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

<span data-ttu-id="679eb-163">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **multiValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="679eb-163">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="679eb-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="679eb-164">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="679eb-165">Код отклика</span><span class="sxs-lookup"><span data-stu-id="679eb-165">Response code</span></span>
<span data-ttu-id="679eb-166">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="679eb-166">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="679eb-167">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="679eb-167">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="679eb-168">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="679eb-168">Response body</span></span>

<span data-ttu-id="679eb-p107">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-p107">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="679eb-p108">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="679eb-p108">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="679eb-173">Пример</span><span class="sxs-lookup"><span data-stu-id="679eb-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="679eb-174">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="679eb-174">Request 1</span></span>

<span data-ttu-id="679eb-p109">В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="679eb-p109">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="679eb-178">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="679eb-178">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="679eb-179">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="679eb-179">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="679eb-180">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="679eb-180">Response 1</span></span>

<span data-ttu-id="679eb-p110">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user_post_events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="679eb-p110">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="679eb-183">Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-183">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="679eb-184">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="679eb-184">Request 2</span></span>

<span data-ttu-id="679eb-p111">Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="679eb-p111">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="679eb-188">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="679eb-188">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="679eb-189">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="679eb-189">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="679eb-190">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="679eb-190">Response 2</span></span>

<span data-ttu-id="679eb-p112">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message_update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="679eb-p112">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="679eb-193">Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="679eb-193">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


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




