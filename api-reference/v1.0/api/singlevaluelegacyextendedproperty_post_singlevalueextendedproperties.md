# <a name="create-single-value-extended-property"></a><span data-ttu-id="15ec6-101">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="15ec6-101">Create single-value extended property</span></span>

<span data-ttu-id="15ec6-102">Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="15ec6-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="15ec6-103">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="15ec6-103">The following user resources are supported:</span></span>

- <span data-ttu-id="15ec6-104">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="15ec6-104">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="15ec6-105">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="15ec6-105">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="15ec6-106">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-106">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="15ec6-107">событие</span><span class="sxs-lookup"><span data-stu-id="15ec6-107">event</span></span>](../resources/event.md)
- [<span data-ttu-id="15ec6-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="15ec6-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="15ec6-109">message</span><span class="sxs-lookup"><span data-stu-id="15ec6-109">message</span></span>](../resources/message.md)

<span data-ttu-id="15ec6-110">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="15ec6-110">As well as the following group resources:</span></span>

- <span data-ttu-id="15ec6-111">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="15ec6-111">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="15ec6-112">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="15ec6-112">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="15ec6-113">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="15ec6-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="15ec6-114">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="15ec6-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15ec6-115">Permissions</span></span>
<span data-ttu-id="15ec6-116">В зависимости от ресурса при создании расширенные свойства в и введите (делегированные или приложения) вы запроса на разрешение, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="15ec6-116">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="15ec6-117">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-117">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="15ec6-118">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="15ec6-118">Supported resource</span></span> | <span data-ttu-id="15ec6-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15ec6-119">Delegated (work or school account)</span></span> | <span data-ttu-id="15ec6-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15ec6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ec6-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="15ec6-121">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="15ec6-122">calendar</span><span class="sxs-lookup"><span data-stu-id="15ec6-122">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="15ec6-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="15ec6-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-124">Calendars.ReadWrite</span></span> | <span data-ttu-id="15ec6-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-125">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="15ec6-126">контакт</span><span class="sxs-lookup"><span data-stu-id="15ec6-126">contact</span></span>](../resources/contact.md) | <span data-ttu-id="15ec6-127">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-127">Contacts.ReadWrite</span></span> | <span data-ttu-id="15ec6-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-128">Contacts.ReadWrite</span></span> | <span data-ttu-id="15ec6-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-129">Contacts.ReadWrite</span></span> |
| <span data-ttu-id="15ec6-130">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-130">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="15ec6-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="15ec6-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="15ec6-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="15ec6-134">event</span><span class="sxs-lookup"><span data-stu-id="15ec6-134">event</span></span>](../resources/event.md) | <span data-ttu-id="15ec6-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-135">Calendars.ReadWrite</span></span> | <span data-ttu-id="15ec6-136">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-136">Calendars.ReadWrite</span></span> |  <span data-ttu-id="15ec6-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-137">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="15ec6-138">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="15ec6-138">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="15ec6-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ec6-139">Group.ReadWrite.All</span></span> | <span data-ttu-id="15ec6-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-140">Not supported</span></span> | <span data-ttu-id="15ec6-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-141">Not supported</span></span> |
| <span data-ttu-id="15ec6-142">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="15ec6-142">group [event](../resources/event.md)</span></span> | <span data-ttu-id="15ec6-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ec6-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="15ec6-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-144">Not supported</span></span> | <span data-ttu-id="15ec6-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-145">Not supported</span></span> |
| <span data-ttu-id="15ec6-146">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="15ec6-146">group [post](../resources/post.md)</span></span> | <span data-ttu-id="15ec6-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ec6-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="15ec6-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-148">Not supported</span></span> | <span data-ttu-id="15ec6-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15ec6-149">Not supported</span></span> |
| [<span data-ttu-id="15ec6-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="15ec6-150">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="15ec6-151">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-151">Mail.ReadWrite</span></span> | <span data-ttu-id="15ec6-152">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-152">Mail.ReadWrite</span></span> | <span data-ttu-id="15ec6-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-153">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="15ec6-154">message</span><span class="sxs-lookup"><span data-stu-id="15ec6-154">message</span></span>](../resources/message.md) | <span data-ttu-id="15ec6-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-155">Mail.ReadWrite</span></span> | <span data-ttu-id="15ec6-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-156">Mail.ReadWrite</span></span> | <span data-ttu-id="15ec6-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ec6-157">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ec6-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15ec6-158">HTTP request</span></span>
<span data-ttu-id="15ec6-159">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="15ec6-159">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="15ec6-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="15ec6-163">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="15ec6-163">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="15ec6-164">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="15ec6-164">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="15ec6-165">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="15ec6-165">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="15ec6-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15ec6-166">Request headers</span></span>
| <span data-ttu-id="15ec6-167">Имя</span><span class="sxs-lookup"><span data-stu-id="15ec6-167">Name</span></span>       | <span data-ttu-id="15ec6-168">Значение</span><span class="sxs-lookup"><span data-stu-id="15ec6-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="15ec6-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15ec6-169">Authorization</span></span> | <span data-ttu-id="15ec6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15ec6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15ec6-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15ec6-172">Content-Type</span></span> | <span data-ttu-id="15ec6-173">application/json</span><span class="sxs-lookup"><span data-stu-id="15ec6-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="15ec6-174">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15ec6-174">Request body</span></span>

<span data-ttu-id="15ec6-175">Предоставьте тело JSON каждого объекта [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) в свойстве коллекции **singleValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="15ec6-175">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="15ec6-176">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ec6-176">Property</span></span>|<span data-ttu-id="15ec6-177">Тип</span><span class="sxs-lookup"><span data-stu-id="15ec6-177">Type</span></span>|<span data-ttu-id="15ec6-178">Описание</span><span class="sxs-lookup"><span data-stu-id="15ec6-178">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="15ec6-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="15ec6-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="15ec6-180">Коллекция [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)</span><span class="sxs-lookup"><span data-stu-id="15ec6-180">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="15ec6-181">Массив из одного или нескольких расширенных свойств с одним значением.</span><span class="sxs-lookup"><span data-stu-id="15ec6-181">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="15ec6-182">id</span><span class="sxs-lookup"><span data-stu-id="15ec6-182">id</span></span>|<span data-ttu-id="15ec6-183">Строка</span><span class="sxs-lookup"><span data-stu-id="15ec6-183">String</span></span>|<span data-ttu-id="15ec6-p104">Чтобы идентифицировать свойства в коллекции **singleValueExtendedProperties**, для каждого из них укажите этот параметр. Свойство должно быть одного из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="15ec6-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="15ec6-188">значение</span><span class="sxs-lookup"><span data-stu-id="15ec6-188">value</span></span>|<span data-ttu-id="15ec6-189">строка</span><span class="sxs-lookup"><span data-stu-id="15ec6-189">string</span></span>|<span data-ttu-id="15ec6-p105">Для каждого свойства из коллекции **singleValueExtendedProperties** следует указать значение. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="15ec6-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="15ec6-192">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **singleValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ec6-192">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="15ec6-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ec6-193">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="15ec6-194">Код отклика</span><span class="sxs-lookup"><span data-stu-id="15ec6-194">Response code</span></span>
<span data-ttu-id="15ec6-195">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="15ec6-195">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="15ec6-196">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="15ec6-196">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="15ec6-197">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="15ec6-197">Response body</span></span>

<span data-ttu-id="15ec6-p106">При создании расширенного свойства отклик будет включать только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы отобразить только что созданное расширенное свойство, [примените к экземпляру, содержащему это расширенное свойство, параметр $expand](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="15ec6-200">Когда вы создаете расширенное свойство в _новом_ экземпляре [group post](../resources/post.md) при ответе на беседу или публикацию, отклик будет включать только код отклика, но не новую публикацию или расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="15ec6-200">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="15ec6-201">Пример</span><span class="sxs-lookup"><span data-stu-id="15ec6-201">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="15ec6-202">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="15ec6-202">Request 1</span></span>

<span data-ttu-id="15ec6-p107">Первый пример показывает создание нового события и расширенного свойства с одним значением с помощью одной и той же операции POST. Помимо свойств, которые вы обычно указываете для нового события, тело запроса включает коллекцию **singleValueExtendedProperties**, которая содержит одно расширенное свойство с одним значением, и следующие данные для этого свойства:</span><span class="sxs-lookup"><span data-stu-id="15ec6-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="15ec6-205">**id** (указывает тип свойства как `String`), GUID и свойство `Fun`.</span><span class="sxs-lookup"><span data-stu-id="15ec6-205">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="15ec6-206">**value** (указывает `Food` как значение свойства `Fun`).</span><span class="sxs-lookup"><span data-stu-id="15ec6-206">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

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

##### <a name="response-1"></a><span data-ttu-id="15ec6-207">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="15ec6-207">Response 1</span></span>

<span data-ttu-id="15ec6-p108">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user_post_events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="15ec6-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="15ec6-210">Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-210">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="15ec6-211">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="15ec6-211">Request 2</span></span>

<span data-ttu-id="15ec6-p109">Второй пример показывает создание расширенного свойства с одним значением для указанного существующего сообщения. Это расширенное свойство — единственный элемент в массиве **singleValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="15ec6-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="15ec6-215">**id** (указывает тип свойства как `String`), GUID и свойство `Color`.</span><span class="sxs-lookup"><span data-stu-id="15ec6-215">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="15ec6-216">**value** (указывает `Green` как значение свойства `Color`).</span><span class="sxs-lookup"><span data-stu-id="15ec6-216">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=

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

##### <a name="response-2"></a><span data-ttu-id="15ec6-217">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="15ec6-217">Response 2</span></span>

<span data-ttu-id="15ec6-p110">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message_update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="15ec6-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="15ec6-220">Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="15ec6-220">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

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

