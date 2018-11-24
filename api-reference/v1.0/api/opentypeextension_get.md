# <a name="get-open-extension"></a><span data-ttu-id="783aa-101">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="783aa-101">Get open extension</span></span>

<span data-ttu-id="783aa-102">Получение открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)), определенного по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="783aa-102">Get an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="783aa-103">В приведенной ниже таблице перечислены три сценария, согласно которым можно получить открытое расширение из поддерживаемого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="783aa-103">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="783aa-104">**Сценарий GET**</span><span class="sxs-lookup"><span data-stu-id="783aa-104">**GET scenario**</span></span>|<span data-ttu-id="783aa-105">**Поддерживаемые ресурсы**</span><span class="sxs-lookup"><span data-stu-id="783aa-105">**Supported resources**</span></span>|<span data-ttu-id="783aa-106">**Текст ответа**</span><span class="sxs-lookup"><span data-stu-id="783aa-106">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="783aa-107">Получение определенного расширения из экземпляра известного ресурса.</span><span class="sxs-lookup"><span data-stu-id="783aa-107">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="783aa-108">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="783aa-108">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="783aa-109">Только открытое расширение.</span><span class="sxs-lookup"><span data-stu-id="783aa-109">Open extension only.</span></span>|
|<span data-ttu-id="783aa-110">Получение экземпляра известного ресурса, дополненного определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-110">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="783aa-111">Device, event, group, group event, group post, message, organization, personal contact, user</span><span class="sxs-lookup"><span data-stu-id="783aa-111">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="783aa-112">Экземпляр известного ресурса, дополненный открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-112">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="783aa-113">Поиск экземпляров ресурсов и их дополнение определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-113">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="783aa-114">Event, group event, group post, message, personal contact</span><span class="sxs-lookup"><span data-stu-id="783aa-114">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="783aa-115">Экземпляры ресурса, дополненные открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-115">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="783aa-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="783aa-116">Permissions</span></span>

<span data-ttu-id="783aa-117">В зависимости от ресурсов, содержащий данное расширение имени файла и разрешение типа (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="783aa-117">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="783aa-118">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="783aa-118">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="783aa-119">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="783aa-119">Supported resource</span></span> | <span data-ttu-id="783aa-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="783aa-120">Delegated (work or school account)</span></span> | <span data-ttu-id="783aa-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="783aa-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="783aa-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="783aa-122">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="783aa-123">device</span><span class="sxs-lookup"><span data-stu-id="783aa-123">device</span></span>](../resources/device.md) | <span data-ttu-id="783aa-124">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-124">Directory.Read.All</span></span> | <span data-ttu-id="783aa-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-125">Not supported</span></span> | <span data-ttu-id="783aa-126">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="783aa-126">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="783aa-127">event</span><span class="sxs-lookup"><span data-stu-id="783aa-127">event</span></span>](../resources/event.md) | <span data-ttu-id="783aa-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-128">Calendars.Read</span></span> | <span data-ttu-id="783aa-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-129">Calendars.Read</span></span> | <span data-ttu-id="783aa-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-130">Calendars.Read</span></span> |
| [<span data-ttu-id="783aa-131">group</span><span class="sxs-lookup"><span data-stu-id="783aa-131">group</span></span>](../resources/group.md) | <span data-ttu-id="783aa-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-132">Group.Read.All</span></span> | <span data-ttu-id="783aa-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-133">Not supported</span></span> | <span data-ttu-id="783aa-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-134">Group.Read.All</span></span> |
| <span data-ttu-id="783aa-135">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="783aa-135">[group event](../resources/event.md)</span></span> | <span data-ttu-id="783aa-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-136">Group.Read.All</span></span> | <span data-ttu-id="783aa-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-137">Not supported</span></span> | <span data-ttu-id="783aa-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-138">Not supported</span></span> |
| <span data-ttu-id="783aa-139">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="783aa-139">[group post](../resources/post.md)</span></span> | <span data-ttu-id="783aa-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-140">Group.Read.All</span></span> | <span data-ttu-id="783aa-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-141">Not supported</span></span> | <span data-ttu-id="783aa-142">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-142">Group.Read.All</span></span> |
| [<span data-ttu-id="783aa-143">message</span><span class="sxs-lookup"><span data-stu-id="783aa-143">message</span></span>](../resources/message.md) | <span data-ttu-id="783aa-144">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-144">Mail.Read</span></span> | <span data-ttu-id="783aa-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-145">Mail.Read</span></span> | <span data-ttu-id="783aa-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-146">Mail.Read</span></span> | 
| [<span data-ttu-id="783aa-147">organization</span><span class="sxs-lookup"><span data-stu-id="783aa-147">organization</span></span>](../resources/organization.md) | <span data-ttu-id="783aa-148">User.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-148">User.Read</span></span> | <span data-ttu-id="783aa-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-149">Not supported</span></span> | <span data-ttu-id="783aa-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="783aa-150">Not supported</span></span> |
| <span data-ttu-id="783aa-151">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="783aa-151">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="783aa-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-152">Contacts.Read</span></span> | <span data-ttu-id="783aa-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-153">Contacts.Read</span></span> | <span data-ttu-id="783aa-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-154">Contacts.Read</span></span> |
| [<span data-ttu-id="783aa-155">user</span><span class="sxs-lookup"><span data-stu-id="783aa-155">user</span></span>](../resources/user.md) | <span data-ttu-id="783aa-156">User.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-156">User.Read</span></span> | <span data-ttu-id="783aa-157">User.Read</span><span class="sxs-lookup"><span data-stu-id="783aa-157">User.Read</span></span> | <span data-ttu-id="783aa-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="783aa-158">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="783aa-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="783aa-159">HTTP request</span></span>

<span data-ttu-id="783aa-160">В этом разделе указан синтаксис для каждого из трех перечисленных выше сценариев с `GET`.</span><span class="sxs-lookup"><span data-stu-id="783aa-160">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="783aa-161">Получение определенного расширения в известном экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="783aa-161">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="783aa-162">Используйте такой же запрос REST, что и при получении экземпляра ресурса, и определите расширение с помощью свойства навигации **extensions** этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="783aa-162">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="783aa-163">Получение известного экземпляра ресурса с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="783aa-163">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="783aa-p102">Для типов ресурса, таких как event, group event, group post, message, personal contact, можно использовать такой же запрос REST, что и при получении экземпляра ресурса. Найдите расширение, соответствующее заданному свойству **id**, и дополните экземпляр расширением. Отклик включает большинство свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="783aa-p102">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="783aa-166">Для типов ресурса device, group, organization и user также необходимо использовать параметр `$select`, чтобы включить свойство **id** и другие свойства, которые необходимо получить из экземпляра ресурса:</span><span class="sxs-lookup"><span data-stu-id="783aa-166">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="783aa-167">Фильтрация экземпляров ресурсов с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="783aa-167">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="783aa-168">Используйте такой же запрос REST, что и при получении коллекции поддерживаемого ресурса, отфильтруйте в коллекции экземпляры, содержащие расширение с соответствующим свойством **id**, и дополните эти экземпляры расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-168">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="783aa-p103">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения коллекции или экземпляров ресурсов, чье расширение нужно получить. Все другие варианты синтаксиса, позволяющие определить эти коллекции или экземпляры ресурсов, поддерживают получение открытых расширений этих экземпляров или коллекций подобным образом.</span><span class="sxs-lookup"><span data-stu-id="783aa-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="783aa-171">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="783aa-171">Path parameters</span></span>
|<span data-ttu-id="783aa-172">Параметр</span><span class="sxs-lookup"><span data-stu-id="783aa-172">Parameter</span></span>|<span data-ttu-id="783aa-173">Тип</span><span class="sxs-lookup"><span data-stu-id="783aa-173">Type</span></span>|<span data-ttu-id="783aa-174">Описание</span><span class="sxs-lookup"><span data-stu-id="783aa-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="783aa-175">Id</span><span class="sxs-lookup"><span data-stu-id="783aa-175">Id</span></span>|<span data-ttu-id="783aa-176">string</span><span class="sxs-lookup"><span data-stu-id="783aa-176">string</span></span>|<span data-ttu-id="783aa-p104">Заполнитель уникального идентификатора для объекта в соответствующей коллекции, например сообщения, события или контакта. Обязательный. Не следует путать его со свойством **id** объекта **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="783aa-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="783aa-180">extensionId</span><span class="sxs-lookup"><span data-stu-id="783aa-180">extensionId</span></span>|<span data-ttu-id="783aa-181">string</span><span class="sxs-lookup"><span data-stu-id="783aa-181">string</span></span>|<span data-ttu-id="783aa-p105">Заполнитель имени расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полного имени, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве **id** при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="783aa-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="783aa-185">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="783aa-185">Optional query parameters</span></span>

<span data-ttu-id="783aa-186">Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке `$filter`.</span><span class="sxs-lookup"><span data-stu-id="783aa-186">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="783aa-187">Имя</span><span class="sxs-lookup"><span data-stu-id="783aa-187">Name</span></span>|<span data-ttu-id="783aa-188">Значение</span><span class="sxs-lookup"><span data-stu-id="783aa-188">Value</span></span>|<span data-ttu-id="783aa-189">Описание</span><span class="sxs-lookup"><span data-stu-id="783aa-189">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="783aa-190">$filter</span><span class="sxs-lookup"><span data-stu-id="783aa-190">$filter</span></span>|<span data-ttu-id="783aa-191">string</span><span class="sxs-lookup"><span data-stu-id="783aa-191">string</span></span>|<span data-ttu-id="783aa-192">Возвращает расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="783aa-192">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="783aa-193">$filter с **любым** оператором</span><span class="sxs-lookup"><span data-stu-id="783aa-193">$filter with **any** operator</span></span>|<span data-ttu-id="783aa-194">string</span><span class="sxs-lookup"><span data-stu-id="783aa-194">string</span></span>|<span data-ttu-id="783aa-195">Возвращает экземпляры коллекции ресурсов, содержащие расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="783aa-195">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="783aa-196">$expand</span><span class="sxs-lookup"><span data-stu-id="783aa-196">$expand</span></span>|<span data-ttu-id="783aa-197">string</span><span class="sxs-lookup"><span data-stu-id="783aa-197">string</span></span>|<span data-ttu-id="783aa-198">Дополняет экземпляр ресурса расширением.</span><span class="sxs-lookup"><span data-stu-id="783aa-198">Expands a resource instance to include an extension.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="783aa-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="783aa-199">Request headers</span></span>
| <span data-ttu-id="783aa-200">Имя</span><span class="sxs-lookup"><span data-stu-id="783aa-200">Name</span></span>       | <span data-ttu-id="783aa-201">Значение</span><span class="sxs-lookup"><span data-stu-id="783aa-201">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="783aa-202">Авторизация</span><span class="sxs-lookup"><span data-stu-id="783aa-202">Authorization</span></span> | <span data-ttu-id="783aa-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="783aa-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="783aa-205">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="783aa-205">Request body</span></span>
<span data-ttu-id="783aa-206">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="783aa-206">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="783aa-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="783aa-207">Response</span></span>

<span data-ttu-id="783aa-p107">В случае успеха этот метод возвращает код отклика `200 OK` и объект [openTypeExtension](../resources/opentypeextension.md) в тексте отклика. Точный текст отклика зависит от запроса GET.</span><span class="sxs-lookup"><span data-stu-id="783aa-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="783aa-210">Пример</span><span class="sxs-lookup"><span data-stu-id="783aa-210">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="783aa-211">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="783aa-211">Request 1</span></span>

<span data-ttu-id="783aa-p108">В первом примере показаны 2 способа обращения к расширению и получение расширения в указанном сообщении. Отклик не зависит от того, как вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="783aa-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="783aa-214">По имени:</span><span class="sxs-lookup"><span data-stu-id="783aa-214">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="783aa-215">По идентификатору (полному имени):</span><span class="sxs-lookup"><span data-stu-id="783aa-215">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="783aa-216">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="783aa-216">Response 1</span></span>
<span data-ttu-id="783aa-217">Ниже представлен отклик для первого примера.</span><span class="sxs-lookup"><span data-stu-id="783aa-217">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="783aa-218">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="783aa-218">Request 2</span></span>

<span data-ttu-id="783aa-219">Во втором примере показано, как сослаться на расширение по его имени и получить расширение в указанном событии группы.</span><span class="sxs-lookup"><span data-stu-id="783aa-219">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```

#### <a name="response-2"></a><span data-ttu-id="783aa-220">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="783aa-220">Response 2</span></span>

<span data-ttu-id="783aa-221">Ниже представлен отклик из второго примера.</span><span class="sxs-lookup"><span data-stu-id="783aa-221">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="783aa-222">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="783aa-222">Request 3</span></span>

<span data-ttu-id="783aa-p109">В третьем примере показано, как получить и дополнить указанное сообщение, добавив расширение, возвращенное из фильтра. Фильтр возвращает расширение, свойство **id** которого совпадает с полным именем.</span><span class="sxs-lookup"><span data-stu-id="783aa-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="783aa-225">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="783aa-225">Response 3</span></span>

<span data-ttu-id="783aa-p110">Ниже представлен отклик из третьего примера. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="783aa-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="783aa-229">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="783aa-229">Request 4</span></span>

<span data-ttu-id="783aa-230">В четвертом примере показано, как сослаться на расширение по его полному имени и получить расширение в указанной записи группы.</span><span class="sxs-lookup"><span data-stu-id="783aa-230">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="783aa-231">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="783aa-231">Response 4</span></span>

<span data-ttu-id="783aa-232">Ниже представлен отклик из четвертого примера.</span><span class="sxs-lookup"><span data-stu-id="783aa-232">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="783aa-233">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="783aa-233">Request 5</span></span>

<span data-ttu-id="783aa-p111">В пятом примере показано, как найти в почтовом ящике вошедшего пользователя сообщения с расширениями, соответствующими фильтру, и дополнить их расширением. Фильтр возвращает расширения, свойство **id** которых совпадает с именем расширения `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="783aa-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="783aa-236">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="783aa-236">Response 5</span></span>

<span data-ttu-id="783aa-237">В этом отклике для пятого примера почтовый ящик пользователя содержит только одно сообщение, свойство **id** которого имеет значение `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="783aa-237">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="783aa-p112">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="783aa-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/opentypeextension_get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get_opentypeextension_1, get_opentypeextension_2, get_opentypeextension_3, get_opentypeextension_5
            Unmapped tables:
        Get open extension - Unknown, Permissions - AuthScopes, Path parameters - PathParameters, Optional query parameters - PathParameters, Request headers - HttpHeaders"
  ],
  "tocPath": ""
}-->
