# <a name="get-contact"></a><span data-ttu-id="f8501-101">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="f8501-101">Get contact</span></span>

<span data-ttu-id="f8501-102">Получение свойств и связей объекта контакта.</span><span class="sxs-lookup"><span data-stu-id="f8501-102">Retrieve the properties and relationships of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8501-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8501-103">Permissions</span></span>
<span data-ttu-id="f8501-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8501-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8501-106">Permission type</span></span>      | <span data-ttu-id="f8501-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8501-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8501-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8501-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f8501-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8501-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f8501-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8501-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8501-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8501-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f8501-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8501-112">Application</span></span> | <span data-ttu-id="f8501-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8501-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8501-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8501-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f8501-115">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f8501-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="f8501-116">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="f8501-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="f8501-p102">[Контакт](../resources/contact.md), содержащийся в дочерней папке объекта [contactFolder](../resources/mailfolder.md). В приведенном ниже примере показан один уровень вложенности, но контакт может храниться в папке, вложенной в дочернюю папку и т. д.</span><span class="sxs-lookup"><span data-stu-id="f8501-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8501-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f8501-119">Optional query parameters</span></span>
|<span data-ttu-id="f8501-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f8501-120">Name</span></span>|<span data-ttu-id="f8501-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8501-121">Value</span></span>|<span data-ttu-id="f8501-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f8501-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="f8501-123">$expand</span><span class="sxs-lookup"><span data-stu-id="f8501-123">$expand</span></span>|<span data-ttu-id="f8501-124">string</span><span class="sxs-lookup"><span data-stu-id="f8501-124">string</span></span>|<span data-ttu-id="f8501-p103">Разделенный запятыми список связей, развертываемых и включаемых в ответ. Поддерживаемые имена представлены в таблице связей объекта [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="f8501-p103">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="f8501-127">$select</span><span class="sxs-lookup"><span data-stu-id="f8501-127">$select</span></span>|<span data-ttu-id="f8501-128">string</span><span class="sxs-lookup"><span data-stu-id="f8501-128">string</span></span>|<span data-ttu-id="f8501-129">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="f8501-129">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f8501-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8501-130">Request headers</span></span>
| <span data-ttu-id="f8501-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8501-131">Header</span></span>       | <span data-ttu-id="f8501-132">Значение</span><span class="sxs-lookup"><span data-stu-id="f8501-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8501-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8501-133">Authorization</span></span>  | <span data-ttu-id="f8501-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8501-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8501-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8501-136">Request body</span></span>
<span data-ttu-id="f8501-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8501-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8501-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8501-138">Response</span></span>

<span data-ttu-id="f8501-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8501-139">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8501-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f8501-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8501-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8501-141">Request</span></span>
<span data-ttu-id="f8501-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8501-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="f8501-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8501-143">Response</span></span>
<span data-ttu-id="f8501-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8501-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
