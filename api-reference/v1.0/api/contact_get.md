# <a name="get-contact"></a><span data-ttu-id="41fde-101">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="41fde-101">Get contact</span></span>

<span data-ttu-id="41fde-102">Получение свойств и связей объекта contact.</span><span class="sxs-lookup"><span data-stu-id="41fde-102">Retrieve the properties and relationships of a contact object.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="41fde-103">Получение контактов из папки контактов другого пользователя</span><span class="sxs-lookup"><span data-stu-id="41fde-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="41fde-104">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить контакты из папки контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="41fde-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="41fde-105">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="41fde-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="41fde-106">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="41fde-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="41fde-107">Предположим, что другой пользователь (Garth) поделился своей папкой контактов с Никитой.</span><span class="sxs-lookup"><span data-stu-id="41fde-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="41fde-108">Вы можете получить контакт из этой общей папки, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="41fde-108">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

<span data-ttu-id="41fde-109">Эта возможность применяется для всех поддерживаемых операций GET над контактами для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="41fde-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="41fde-110">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="41fde-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="41fde-111">Если пользователь Garth не поделился своей папкой контактов с Никитой и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="41fde-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="41fde-112">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить контакт в папке контактов пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="41fde-112">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
```

<span data-ttu-id="41fde-113">Эта возможность доступна только в операциях GET для:</span><span class="sxs-lookup"><span data-stu-id="41fde-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="41fde-114">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="41fde-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="41fde-115">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="41fde-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="41fde-116">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="41fde-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="41fde-117">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="41fde-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="41fde-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41fde-118">Permissions</span></span>
<span data-ttu-id="41fde-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="41fde-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="41fde-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41fde-121">Permission type</span></span>      | <span data-ttu-id="41fde-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41fde-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41fde-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41fde-123">Delegated (work or school account)</span></span> | <span data-ttu-id="41fde-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fde-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="41fde-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41fde-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41fde-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fde-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="41fde-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41fde-127">Application</span></span> | <span data-ttu-id="41fde-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fde-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="41fde-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41fde-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="41fde-130">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="41fde-130">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="41fde-131">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="41fde-131">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="41fde-p106">[Контакт](../resources/contact.md), содержащийся в дочерней папке объекта [contactFolder](../resources/mailfolder.md). В приведенном ниже примере показан один уровень вложенности, но контакт может храниться в папке, вложенной в дочернюю папку и т. д.</span><span class="sxs-lookup"><span data-stu-id="41fde-p106">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41fde-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41fde-134">Optional query parameters</span></span>
|<span data-ttu-id="41fde-135">Имя</span><span class="sxs-lookup"><span data-stu-id="41fde-135">Name</span></span>|<span data-ttu-id="41fde-136">Значение</span><span class="sxs-lookup"><span data-stu-id="41fde-136">Value</span></span>|<span data-ttu-id="41fde-137">Описание</span><span class="sxs-lookup"><span data-stu-id="41fde-137">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="41fde-138">$expand</span><span class="sxs-lookup"><span data-stu-id="41fde-138">$expand</span></span>|<span data-ttu-id="41fde-139">string</span><span class="sxs-lookup"><span data-stu-id="41fde-139">string</span></span>|<span data-ttu-id="41fde-p107">Разделенный запятыми список связей, развертываемых и включаемых в ответ. Поддерживаемые имена представлены в таблице связей объекта [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="41fde-p107">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="41fde-142">$select</span><span class="sxs-lookup"><span data-stu-id="41fde-142">$select</span></span>|<span data-ttu-id="41fde-143">string</span><span class="sxs-lookup"><span data-stu-id="41fde-143">string</span></span>|<span data-ttu-id="41fde-144">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="41fde-144">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="41fde-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41fde-145">Request headers</span></span>
| <span data-ttu-id="41fde-146">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41fde-146">Header</span></span>       | <span data-ttu-id="41fde-147">Значение</span><span class="sxs-lookup"><span data-stu-id="41fde-147">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41fde-148">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41fde-148">Authorization</span></span>  | <span data-ttu-id="41fde-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41fde-p108">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41fde-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41fde-151">Request body</span></span>
<span data-ttu-id="41fde-152">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41fde-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41fde-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="41fde-153">Response</span></span>

<span data-ttu-id="41fde-154">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41fde-154">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41fde-155">Пример</span><span class="sxs-lookup"><span data-stu-id="41fde-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41fde-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="41fde-156">Request</span></span>
<span data-ttu-id="41fde-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41fde-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="41fde-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="41fde-158">Response</span></span>
<span data-ttu-id="41fde-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41fde-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
