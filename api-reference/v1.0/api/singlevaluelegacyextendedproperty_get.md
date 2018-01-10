# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="56b3f-101">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="56b3f-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="56b3f-102">Получение экземпляров ресурса, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="56b3f-p101">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством. На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="56b3f-p102">С помощью параметра запроса `$filter` вы можете получить все экземпляры указанного ресурса, которые содержат расширенное свойство, соответствующее фильтру для свойств **id** и **value**. Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="56b3f-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="56b3f-107">The following user resources are supported:</span></span>

- <span data-ttu-id="56b3f-108">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="56b3f-108">[message](../resources/message.md)</span></span>
- <span data-ttu-id="56b3f-109">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="56b3f-109">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="56b3f-110">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="56b3f-110">[event](../resources/event.md)</span></span>
- <span data-ttu-id="56b3f-111">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="56b3f-111">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="56b3f-112">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="56b3f-112">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="56b3f-113">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="56b3f-113">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="56b3f-114">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="56b3f-114">As well as the following group resources:</span></span>

- <span data-ttu-id="56b3f-115">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="56b3f-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="56b3f-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="56b3f-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="56b3f-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="56b3f-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="56b3f-118">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="56b3f-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="56b3f-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56b3f-119">Permissions</span></span>
<span data-ttu-id="56b3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, который вы получаете). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56b3f-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="56b3f-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="56b3f-122">Mail.Read</span></span>
- <span data-ttu-id="56b3f-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="56b3f-123">Calendars.Read</span></span>
- <span data-ttu-id="56b3f-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="56b3f-124">Contacts.Read</span></span>
- <span data-ttu-id="56b3f-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="56b3f-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="56b3f-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56b3f-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="56b3f-127">Запрос GET на получение экземпляра ресурса с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="56b3f-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="56b3f-p104">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое соответствует фильтру по свойству **id**. Убедитесь, что вы применяете [кодировку URL]((http://www.w3schools.com/tags/ref_urlencode.asp)) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding]((http://www.w3schools.com/tags/ref_urlencode.asp)) to the space characters in the filter string.</span></span>

<span data-ttu-id="56b3f-130">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="56b3f-131">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="56b3f-132">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="56b3f-133">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="56b3f-134">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="56b3f-135">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="56b3f-136">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="56b3f-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="56b3f-137">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="56b3f-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="56b3f-138">Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`</span><span class="sxs-lookup"><span data-stu-id="56b3f-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="56b3f-139">Получение экземпляров поддерживаемого ресурса с расширенным свойством, соответствующим фильтру для свойств **id** и **value**.</span><span class="sxs-lookup"><span data-stu-id="56b3f-139">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply URL encoding to the following characters in the filter string - forward slash and space.</span></span> <span data-ttu-id="56b3f-140">Применяйте [кодировку URL]((http://www.w3schools.com/tags/ref_urlencode.asp)) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="56b3f-140">Get instances of a supported resource that have the extended property matching a filter on the id and value properties. Make sure you apply [URL encoding]((http://www.w3schools.com/tags/ref_urlencode.asp)) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="56b3f-141">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="56b3f-142">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="56b3f-143">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="56b3f-144">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="56b3f-145">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="56b3f-146">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="56b3f-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="56b3f-147">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="56b3f-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="56b3f-148">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="56b3f-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="56b3f-149">Параметры</span><span class="sxs-lookup"><span data-stu-id="56b3f-149">Parameters</span></span>
|<span data-ttu-id="56b3f-150">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="56b3f-150">**Parameter**</span></span>|<span data-ttu-id="56b3f-151">**Тип**</span><span class="sxs-lookup"><span data-stu-id="56b3f-151">**Type**</span></span>|<span data-ttu-id="56b3f-152">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56b3f-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="56b3f-153">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="56b3f-153">_URL parameters_</span></span>|
|<span data-ttu-id="56b3f-154">id_value</span><span class="sxs-lookup"><span data-stu-id="56b3f-154">id_value</span></span>|<span data-ttu-id="56b3f-155">String</span><span class="sxs-lookup"><span data-stu-id="56b3f-155">String</span></span>|<span data-ttu-id="56b3f-p106">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="56b3f-160">property_value</span><span class="sxs-lookup"><span data-stu-id="56b3f-160">property_value</span></span> |<span data-ttu-id="56b3f-161">String</span><span class="sxs-lookup"><span data-stu-id="56b3f-161">String</span></span>|<span data-ttu-id="56b3f-162">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="56b3f-162">The value of the extended property to match. Required where listed in the HTTP request section.</span></span> <span data-ttu-id="56b3f-163">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="56b3f-163">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="56b3f-164">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="56b3f-164">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="56b3f-165">Примеры см. ниже, в [запросе 3](#request-3).</span><span class="sxs-lookup"><span data-stu-id="56b3f-165">See [request 3](#request-3) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="56b3f-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56b3f-166">Request headers</span></span>
| <span data-ttu-id="56b3f-167">Имя</span><span class="sxs-lookup"><span data-stu-id="56b3f-167">Name</span></span>      |<span data-ttu-id="56b3f-168">Описание</span><span class="sxs-lookup"><span data-stu-id="56b3f-168">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56b3f-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56b3f-169">Authorization</span></span>  | <span data-ttu-id="56b3f-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56b3f-172">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56b3f-172">Request body</span></span>
<span data-ttu-id="56b3f-173">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56b3f-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56b3f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="56b3f-174">Response</span></span>

<span data-ttu-id="56b3f-175">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-175">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="56b3f-176">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="56b3f-176">GET resource instance using `$expand`</span></span>
<span data-ttu-id="56b3f-177">Текст отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="56b3f-177">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="56b3f-178">Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`</span><span class="sxs-lookup"><span data-stu-id="56b3f-178">GET resource instances using `$filter`</span></span>
<span data-ttu-id="56b3f-p109">Текст отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство. Текст отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="56b3f-181">Пример</span><span class="sxs-lookup"><span data-stu-id="56b3f-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="56b3f-182">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="56b3f-182">Request 1</span></span>

<span data-ttu-id="56b3f-p110">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="56b3f-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="56b3f-185">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="56b3f-185">Response 1</span></span>
<span data-ttu-id="56b3f-186">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="56b3f-186">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="56b3f-p111">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="56b3f-189">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="56b3f-189">Request 2</span></span>

<span data-ttu-id="56b3f-190">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="56b3f-190">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span> <span data-ttu-id="56b3f-191">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="56b3f-191">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="56b3f-192">Свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="56b3f-192">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="56b3f-193">Свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-193">Its **value** being the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="56b3f-194">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="56b3f-194">Response 2</span></span>

<span data-ttu-id="56b3f-p113">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user_list_messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="56b3f-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="56b3f-198">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="56b3f-198">Request 3</span></span>

<span data-ttu-id="56b3f-199">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от string.</span><span class="sxs-lookup"><span data-stu-id="56b3f-199">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="56b3f-200">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="56b3f-200">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="56b3f-201">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="56b3f-201">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="56b3f-202">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-202">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="56b3f-203">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-203">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="56b3f-204">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-204">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="56b3f-205">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="56b3f-205">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="56b3f-206">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-206">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="56b3f-207">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="56b3f-207">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="56b3f-208">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="56b3f-208">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-3"></a><span data-ttu-id="56b3f-209">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="56b3f-209">Response 3</span></span>

<span data-ttu-id="56b3f-210">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="56b3f-210">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="56b3f-211">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="56b3f-211">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="56b3f-212">Ответ не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="56b3f-212">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->