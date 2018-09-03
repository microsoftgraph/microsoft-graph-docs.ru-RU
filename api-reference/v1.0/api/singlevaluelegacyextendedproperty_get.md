# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="24e5a-101">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="24e5a-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="24e5a-102">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="24e5a-102">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="24e5a-103">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="24e5a-103">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="24e5a-104">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-104">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="24e5a-105">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-105">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="24e5a-106">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="24e5a-106">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="24e5a-107">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-107">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="24e5a-108">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="24e5a-108">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="24e5a-109">Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="24e5a-109">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="24e5a-110">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="24e5a-110">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="24e5a-111">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="24e5a-111">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="24e5a-112">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="24e5a-112">The following user resources are supported:</span></span>

- <span data-ttu-id="24e5a-113">[[message](../resources/message.md);](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-113">[message](../resources/message.md)</span></span>
- <span data-ttu-id="24e5a-114">[[mailFolder](../resources/mailfolder.md);](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-114">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="24e5a-115">[[event](../resources/event.md);](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-115">[event](../resources/event.md)</span></span>
- <span data-ttu-id="24e5a-116">[[calendar](../resources/calendar.md);](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-116">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="24e5a-117">[[contact](../resources/contact.md);](../resources/contact.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-117">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="24e5a-118">[[contactFolder](../resources/contactfolder.md).](../resources/contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="24e5a-118">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="24e5a-119">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="24e5a-119">As well as the following group resources:</span></span>

- <span data-ttu-id="24e5a-120">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="24e5a-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="24e5a-121">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="24e5a-121">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="24e5a-122">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="24e5a-122">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="24e5a-123">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="24e5a-123">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24e5a-124">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24e5a-124">Permissions</span></span>
<span data-ttu-id="24e5a-p104">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, который вы получаете). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24e5a-p104">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="24e5a-127">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24e5a-127">Mail.Read</span></span>
- <span data-ttu-id="24e5a-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24e5a-128">Calendars.Read</span></span>
- <span data-ttu-id="24e5a-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24e5a-129">Contacts.Read</span></span>
- <span data-ttu-id="24e5a-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24e5a-130">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="24e5a-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24e5a-131">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="24e5a-132">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="24e5a-132">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="24e5a-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="24e5a-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="24e5a-135">Получение экземпляра объекта**message**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-135">Get a **message** instance:</span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24e5a-136">Получение экземпляра объекта **mailFolder**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-136">Get a **mailFolder** instance:</span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24e5a-137">Получение экземпляра объекта **event**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-137">Get an **event** instance:</span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24e5a-138">Получение экземпляра объекта **calendar**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-138">Get a **calendar** instance:</span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24e5a-139">Получение экземпляра объекта **contact**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-139">Get a **contact** instance:</span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24e5a-140">Получение экземпляра объекта **contactFolder**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-140">Get a **contactFolder** instance:</span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24e5a-141">Получение экземпляра объекта **event** для группы: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-141">Get a group **event** instance:</span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24e5a-142">Получение экземпляра объекта **post** для группы: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-142">Get a group **post** instance:</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="24e5a-143">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="24e5a-143">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="24e5a-144">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="24e5a-144">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="24e5a-145">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-145">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="24e5a-146">Применяйте [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="24e5a-146">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="24e5a-147">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="24e5a-147">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="24e5a-148">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="24e5a-148">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="24e5a-149">Получение экземпляров объекта **message**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-149">Get **message** instances:</span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="24e5a-150">Получение экземпляров объекта **mailFolder**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-150">Get **mailFolder** instances:</span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="24e5a-151">Получение экземпляров объекта **event**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-151">Get **event** instances:</span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="24e5a-152">Получение экземпляров объекта **calendar**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-152">Get **calendar** instances:</span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="24e5a-153">Получение экземпляров объекта **contact**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-153">Get **contact** instances:</span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="24e5a-154">Получение экземпляров объекта **contactFolder**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-154">Get **contactFolder** instances:</span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="24e5a-155">Получение экземпляров объекта **event** для группы: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-155">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="24e5a-156">Получение экземпляров объекта **post** для группы: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-156">Get group **post** instances:</span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="24e5a-157">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="24e5a-157">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="24e5a-158">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="24e5a-158">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="24e5a-159">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-159">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="24e5a-160">Применяйте [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="24e5a-160">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="24e5a-161">Получение экземпляров объекта **message**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-161">Get **message** instances:</span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="24e5a-162">Получение экземпляров объекта **event**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-162">Get **event** instances:</span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="24e5a-163">Получение экземпляров объекта **event** для группы: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24e5a-163">Get group **event** instances:</span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="24e5a-164">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="24e5a-164">Path parameters</span></span>
|<span data-ttu-id="24e5a-165">Параметр</span><span class="sxs-lookup"><span data-stu-id="24e5a-165">Parameter</span></span>|<span data-ttu-id="24e5a-166">Тип</span><span class="sxs-lookup"><span data-stu-id="24e5a-166">Type</span></span>|<span data-ttu-id="24e5a-167">Описание</span><span class="sxs-lookup"><span data-stu-id="24e5a-167">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="24e5a-168">id_value</span><span class="sxs-lookup"><span data-stu-id="24e5a-168">id_value</span></span>|<span data-ttu-id="24e5a-169">String</span><span class="sxs-lookup"><span data-stu-id="24e5a-169">String</span></span>|<span data-ttu-id="24e5a-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e5a-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="24e5a-174">property_value</span><span class="sxs-lookup"><span data-stu-id="24e5a-174">property_value</span></span> |<span data-ttu-id="24e5a-175">String</span><span class="sxs-lookup"><span data-stu-id="24e5a-175">String</span></span>|<span data-ttu-id="24e5a-176">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="24e5a-176">The value of the extended property to match.</span></span> <span data-ttu-id="24e5a-177">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="24e5a-177">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="24e5a-178">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="24e5a-178">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="24e5a-179">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="24e5a-179">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="24e5a-180">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24e5a-180">Request headers</span></span>
| <span data-ttu-id="24e5a-181">Имя</span><span class="sxs-lookup"><span data-stu-id="24e5a-181">Name</span></span>      |<span data-ttu-id="24e5a-182">Описание</span><span class="sxs-lookup"><span data-stu-id="24e5a-182">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24e5a-183">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24e5a-183">Authorization</span></span>  | <span data-ttu-id="24e5a-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e5a-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24e5a-186">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24e5a-186">Request body</span></span>
<span data-ttu-id="24e5a-187">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24e5a-187">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e5a-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="24e5a-188">Response</span></span>

<span data-ttu-id="24e5a-189">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-189">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="24e5a-190">Получение экземпляра ресурса с соответствующим расширенным свойством</span><span class="sxs-lookup"><span data-stu-id="24e5a-190">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="24e5a-191">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="24e5a-191">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="24e5a-192">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="24e5a-192">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="24e5a-193">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-193">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="24e5a-194">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-194">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="24e5a-195">Пример</span><span class="sxs-lookup"><span data-stu-id="24e5a-195">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="24e5a-196">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="24e5a-196">Request 1</span></span>

<span data-ttu-id="24e5a-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="24e5a-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="24e5a-199">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="24e5a-199">Response 1</span></span>
<span data-ttu-id="24e5a-200">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="24e5a-200">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="24e5a-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24e5a-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="24e5a-203">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="24e5a-203">Request 2</span></span>

<span data-ttu-id="24e5a-204">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="24e5a-204">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="24e5a-205">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="24e5a-205">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="24e5a-206">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="24e5a-206">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="24e5a-207">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-207">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="24e5a-208">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="24e5a-208">Response 2</span></span>

<span data-ttu-id="24e5a-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user_list_messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="24e5a-212">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="24e5a-212">Request 3</span></span>

<span data-ttu-id="24e5a-213">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="24e5a-213">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="24e5a-214">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="24e5a-214">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="24e5a-215">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="24e5a-215">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="24e5a-216">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-216">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="24e5a-217">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="24e5a-217">Response 3</span></span>

<span data-ttu-id="24e5a-218">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="24e5a-218">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="24e5a-219">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="24e5a-219">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="24e5a-220">Тело отклика такое же, как при [получении коллекции сообщений](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="24e5a-220">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="24e5a-221">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-221">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="24e5a-222">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="24e5a-222">Request 4</span></span>

<span data-ttu-id="24e5a-223">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="24e5a-223">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="24e5a-224">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="24e5a-224">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="24e5a-225">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="24e5a-225">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="24e5a-226">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-226">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="24e5a-227">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-227">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="24e5a-228">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-228">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="24e5a-229">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="24e5a-229">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="24e5a-230">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-230">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="24e5a-231">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="24e5a-231">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="24e5a-232">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="24e5a-232">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="24e5a-233">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="24e5a-233">Response 4</span></span>

<span data-ttu-id="24e5a-234">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="24e5a-234">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="24e5a-235">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user_list_messages.md).</span><span class="sxs-lookup"><span data-stu-id="24e5a-235">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="24e5a-236">Ответ не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="24e5a-236">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->