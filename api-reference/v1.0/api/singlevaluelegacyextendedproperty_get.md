# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="e4a37-101">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e4a37-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="e4a37-102">Получение экземпляров ресурса, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e4a37-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="e4a37-p101">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством. На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="e4a37-p102">С помощью параметра запроса `$filter` вы можете получить все экземпляры указанного ресурса, которые содержат расширенное свойство, соответствующее фильтру для свойств **id** и **value**. Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="e4a37-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="e4a37-107">The following user resources are supported:</span></span>

- <span data-ttu-id="e4a37-108">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="e4a37-108">[message](../resources/message.md)</span></span>
- <span data-ttu-id="e4a37-109">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="e4a37-109">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="e4a37-110">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="e4a37-110">[event](../resources/event.md)</span></span>
- <span data-ttu-id="e4a37-111">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="e4a37-111">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e4a37-112">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="e4a37-112">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="e4a37-113">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e4a37-113">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="e4a37-114">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="e4a37-114">As well as the following group resources:</span></span>

- <span data-ttu-id="e4a37-115">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="e4a37-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="e4a37-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="e4a37-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e4a37-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="e4a37-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="e4a37-118">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e4a37-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a37-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a37-119">Permissions</span></span>
<span data-ttu-id="e4a37-p103">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, который вы получаете). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4a37-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="e4a37-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e4a37-122">Mail.Read</span></span>
- <span data-ttu-id="e4a37-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e4a37-123">Calendars.Read</span></span>
- <span data-ttu-id="e4a37-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e4a37-124">Contacts.Read</span></span>
- <span data-ttu-id="e4a37-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a37-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="e4a37-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4a37-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="e4a37-127">Запрос GET на получение экземпляра ресурса с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="e4a37-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="e4a37-p104">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое соответствует фильтру по свойству **id**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="e4a37-130">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e4a37-131">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e4a37-132">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e4a37-133">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e4a37-134">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e4a37-135">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e4a37-136">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="e4a37-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e4a37-137">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="e4a37-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="e4a37-138">Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`</span><span class="sxs-lookup"><span data-stu-id="e4a37-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="e4a37-p105">Получение экземпляров поддерживаемого ресурса с расширенным свойством, соответствующим фильтру для свойств **id** и **value**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов косой черты и пробела в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p105">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="e4a37-141">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e4a37-142">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e4a37-143">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e4a37-144">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e4a37-145">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e4a37-146">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="e4a37-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e4a37-147">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="e4a37-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e4a37-148">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="e4a37-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="e4a37-149">Параметры</span><span class="sxs-lookup"><span data-stu-id="e4a37-149">Parameters</span></span>
|<span data-ttu-id="e4a37-150">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="e4a37-150">**Parameter**</span></span>|<span data-ttu-id="e4a37-151">**Тип**</span><span class="sxs-lookup"><span data-stu-id="e4a37-151">**Type**</span></span>|<span data-ttu-id="e4a37-152">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4a37-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e4a37-153">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="e4a37-153">_URL parameters_</span></span>|
|<span data-ttu-id="e4a37-154">id_value</span><span class="sxs-lookup"><span data-stu-id="e4a37-154">id_value</span></span>|<span data-ttu-id="e4a37-155">String</span><span class="sxs-lookup"><span data-stu-id="e4a37-155">String</span></span>|<span data-ttu-id="e4a37-p106">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="e4a37-160">property_value</span><span class="sxs-lookup"><span data-stu-id="e4a37-160">property_value</span></span>|<span data-ttu-id="e4a37-161">String</span><span class="sxs-lookup"><span data-stu-id="e4a37-161">String</span></span>|<span data-ttu-id="e4a37-p107">Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e4a37-164">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4a37-164">Request headers</span></span>
| <span data-ttu-id="e4a37-165">Имя</span><span class="sxs-lookup"><span data-stu-id="e4a37-165">Name</span></span>      |<span data-ttu-id="e4a37-166">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a37-166">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4a37-167">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4a37-167">Authorization</span></span>  | <span data-ttu-id="e4a37-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a37-170">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4a37-170">Request body</span></span>
<span data-ttu-id="e4a37-171">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4a37-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a37-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a37-172">Response</span></span>

<span data-ttu-id="e4a37-173">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e4a37-173">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="e4a37-174">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="e4a37-174">GET resource instance using `$expand`</span></span>
<span data-ttu-id="e4a37-175">Текст отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e4a37-175">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="e4a37-176">Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`</span><span class="sxs-lookup"><span data-stu-id="e4a37-176">GET resource instances using `$filter`</span></span>
<span data-ttu-id="e4a37-p109">Текст отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство. Текст отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="e4a37-179">Пример</span><span class="sxs-lookup"><span data-stu-id="e4a37-179">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e4a37-180">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e4a37-180">Request 1</span></span>

<span data-ttu-id="e4a37-p110">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="e4a37-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a><span data-ttu-id="e4a37-183">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="e4a37-183">Response 1</span></span>
<span data-ttu-id="e4a37-184">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="e4a37-184">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="e4a37-p111">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

****

#### <a name="request-2"></a><span data-ttu-id="e4a37-187">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e4a37-187">Request 2</span></span>

<span data-ttu-id="e4a37-p112">Во втором примере показано, как получить сообщения, у которых есть расширенное свойство с одним значением, указанное в фильтре. Фильтр возвращает расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="e4a37-p112">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span>
- <span data-ttu-id="e4a37-190">Параметр **id** совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="e4a37-190">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>
- <span data-ttu-id="e4a37-191">Для параметра **value** задано значение `Green`.</span><span class="sxs-lookup"><span data-stu-id="e4a37-191">Its **value** being `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a><span data-ttu-id="e4a37-192">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e4a37-192">Response 2</span></span>

<span data-ttu-id="e4a37-p113">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user_list_messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e4a37-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->