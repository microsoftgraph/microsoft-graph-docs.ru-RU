# <a name="get-contact"></a><span data-ttu-id="3e916-101">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="3e916-101">Get contact</span></span>

<span data-ttu-id="3e916-102">Получение свойств и связей объекта contact.</span><span class="sxs-lookup"><span data-stu-id="3e916-102">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="3e916-103">Существует два сценария, где приложения можно получить контакт в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e916-103">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="3e916-104">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="3e916-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="3e916-105">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="3e916-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="3e916-106">В разделе [сведения и примеры](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="3e916-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="3e916-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e916-107">Permissions</span></span>
<span data-ttu-id="3e916-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e916-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e916-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e916-110">Permission type</span></span>      | <span data-ttu-id="3e916-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e916-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e916-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e916-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e916-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e916-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e916-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e916-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e916-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e916-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e916-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e916-116">Application</span></span> | <span data-ttu-id="3e916-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e916-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e916-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e916-118">HTTP request</span></span>
<span data-ttu-id="3e916-119"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3e916-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="3e916-120">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="3e916-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="3e916-p103">[Контакт](../resources/contact.md), содержащийся в дочерней папке объекта [contactFolder](../resources/mailfolder.md). В приведенном ниже примере показан один уровень вложенности, но контакт может храниться в папке, вложенной в дочернюю папку и т. д.</span><span class="sxs-lookup"><span data-stu-id="3e916-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e916-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e916-123">Optional query parameters</span></span>
|<span data-ttu-id="3e916-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3e916-124">Name</span></span>|<span data-ttu-id="3e916-125">Значение</span><span class="sxs-lookup"><span data-stu-id="3e916-125">Value</span></span>|<span data-ttu-id="3e916-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3e916-126">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3e916-127">$expand</span><span class="sxs-lookup"><span data-stu-id="3e916-127">$expand</span></span>|<span data-ttu-id="3e916-128">string</span><span class="sxs-lookup"><span data-stu-id="3e916-128">string</span></span>|<span data-ttu-id="3e916-p104">Разделенный запятыми список связей, развертываемых и включаемых в ответ. Поддерживаемые имена представлены в таблице связей объекта [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="3e916-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="3e916-131">$select</span><span class="sxs-lookup"><span data-stu-id="3e916-131">$select</span></span>|<span data-ttu-id="3e916-132">string</span><span class="sxs-lookup"><span data-stu-id="3e916-132">string</span></span>|<span data-ttu-id="3e916-133">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="3e916-133">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3e916-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e916-134">Request headers</span></span>
| <span data-ttu-id="3e916-135">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e916-135">Header</span></span>       | <span data-ttu-id="3e916-136">Значение</span><span class="sxs-lookup"><span data-stu-id="3e916-136">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e916-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e916-137">Authorization</span></span>  | <span data-ttu-id="3e916-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e916-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e916-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e916-140">Request body</span></span>
<span data-ttu-id="3e916-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e916-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e916-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e916-142">Response</span></span>

<span data-ttu-id="3e916-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e916-143">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e916-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3e916-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e916-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e916-145">Request</span></span>
<span data-ttu-id="3e916-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e916-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="3e916-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e916-147">Response</span></span>
<span data-ttu-id="3e916-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3e916-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
