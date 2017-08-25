# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="52f0a-101">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="52f0a-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="52f0a-102">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="52f0a-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="52f0a-p101">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством. На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="52f0a-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="52f0a-105">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="52f0a-105">The following user resources are supported:</span></span>

- <span data-ttu-id="52f0a-106">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="52f0a-106">[message](../resources/message.md)</span></span>
- <span data-ttu-id="52f0a-107">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="52f0a-107">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="52f0a-108">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="52f0a-108">[event](../resources/event.md)</span></span>
- <span data-ttu-id="52f0a-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="52f0a-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="52f0a-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="52f0a-110">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="52f0a-111">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="52f0a-111">[contactFolder](../resources/contactfolder.md)</span></span> 

<span data-ttu-id="52f0a-112">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="52f0a-112">As well as the following group resources:</span></span>

- <span data-ttu-id="52f0a-113">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="52f0a-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="52f0a-114">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="52f0a-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="52f0a-115">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="52f0a-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="52f0a-116">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="52f0a-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f0a-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52f0a-117">Permissions</span></span>
<span data-ttu-id="52f0a-p102">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, который вы получаете). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="52f0a-p102">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="52f0a-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="52f0a-120">Mail.Read</span></span>
- <span data-ttu-id="52f0a-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="52f0a-121">Calendars.Read</span></span>
- <span data-ttu-id="52f0a-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="52f0a-122">Contacts.Read</span></span>
- <span data-ttu-id="52f0a-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="52f0a-123">Group.Read.All</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="52f0a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f0a-124">HTTP request</span></span>

<span data-ttu-id="52f0a-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="52f0a-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="52f0a-127">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-127">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="52f0a-128">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-128">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="52f0a-129">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-129">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="52f0a-130">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-130">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="52f0a-131">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-131">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="52f0a-132">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-132">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="52f0a-133">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="52f0a-133">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="52f0a-134">Получение экземпляра группы **post**:</span><span class="sxs-lookup"><span data-stu-id="52f0a-134">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="parameters"></a><span data-ttu-id="52f0a-135">Параметры</span><span class="sxs-lookup"><span data-stu-id="52f0a-135">Parameters</span></span>
|<span data-ttu-id="52f0a-136">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="52f0a-136">**Parameter**</span></span>|<span data-ttu-id="52f0a-137">**Тип**</span><span class="sxs-lookup"><span data-stu-id="52f0a-137">**Type**</span></span>|<span data-ttu-id="52f0a-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52f0a-138">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52f0a-139">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="52f0a-139">_URL parameters_</span></span>|
|<span data-ttu-id="52f0a-140">id_value</span><span class="sxs-lookup"><span data-stu-id="52f0a-140">id_value</span></span>|<span data-ttu-id="52f0a-141">String</span><span class="sxs-lookup"><span data-stu-id="52f0a-141">String</span></span>|<span data-ttu-id="52f0a-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f0a-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="52f0a-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f0a-146">Request headers</span></span>
| <span data-ttu-id="52f0a-147">Имя</span><span class="sxs-lookup"><span data-stu-id="52f0a-147">Name</span></span>      |<span data-ttu-id="52f0a-148">Описание</span><span class="sxs-lookup"><span data-stu-id="52f0a-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52f0a-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f0a-149">Authorization</span></span>  | <span data-ttu-id="52f0a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f0a-p105">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="52f0a-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f0a-152">Request body</span></span>
<span data-ttu-id="52f0a-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52f0a-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52f0a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f0a-154">Response</span></span>

<span data-ttu-id="52f0a-155">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="52f0a-155">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="52f0a-156">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="52f0a-156">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="52f0a-157">Пример</span><span class="sxs-lookup"><span data-stu-id="52f0a-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52f0a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f0a-158">Request</span></span>
<span data-ttu-id="52f0a-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="52f0a-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="52f0a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f0a-161">Response</span></span>

<span data-ttu-id="52f0a-162">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="52f0a-162">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="52f0a-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="52f0a-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->