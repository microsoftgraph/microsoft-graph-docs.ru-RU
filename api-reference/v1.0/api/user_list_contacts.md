# <a name="list-contacts"></a><span data-ttu-id="479b2-101">Список контактов</span><span class="sxs-lookup"><span data-stu-id="479b2-101">List contacts</span></span>

<span data-ttu-id="479b2-102">В этой статье рассказывается, как получить коллекцию контактов из папки контактов, используемой по умолчанию, для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="479b2-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="479b2-103">Получение контактов из папки контактов другого пользователя</span><span class="sxs-lookup"><span data-stu-id="479b2-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="479b2-104">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить контакты из папки контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="479b2-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="479b2-105">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="479b2-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="479b2-106">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="479b2-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="479b2-107">Предположим, что другой пользователь (Garth) поделился своей папкой контактов с Никитой.</span><span class="sxs-lookup"><span data-stu-id="479b2-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="479b2-108">Вы можете получить контакты из этой общей папки, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="479b2-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="479b2-109">Эта возможность применяется для всех поддерживаемых операций GET над контактами для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="479b2-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="479b2-110">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="479b2-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="479b2-111">Если пользователь Garth не поделился своей папкой контактов с Никитой и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="479b2-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="479b2-112">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить контакты в папке контактов пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="479b2-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="479b2-113">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="479b2-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="479b2-114">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="479b2-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="479b2-115">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="479b2-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="479b2-116">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="479b2-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="479b2-117">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="479b2-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="479b2-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="479b2-118">Permissions</span></span>
<span data-ttu-id="479b2-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="479b2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="479b2-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="479b2-121">Permission type</span></span>      | <span data-ttu-id="479b2-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="479b2-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="479b2-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="479b2-123">Delegated (work or school account)</span></span> | <span data-ttu-id="479b2-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b2-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="479b2-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="479b2-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="479b2-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b2-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="479b2-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="479b2-127">Application</span></span> | <span data-ttu-id="479b2-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="479b2-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="479b2-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="479b2-129">HTTP request</span></span>

<span data-ttu-id="479b2-130">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="479b2-130">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="479b2-131">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="479b2-131">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="479b2-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="479b2-132">Optional query parameters</span></span>
<span data-ttu-id="479b2-133">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="479b2-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="479b2-134">Например, с помощью параметра запроса `$filter` можно фильтровать контакты на основе домена, указанного в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="479b2-134">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="479b2-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="479b2-135">Request headers</span></span>
| <span data-ttu-id="479b2-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="479b2-136">Header</span></span>       | <span data-ttu-id="479b2-137">Значение</span><span class="sxs-lookup"><span data-stu-id="479b2-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="479b2-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="479b2-138">Authorization</span></span>  | <span data-ttu-id="479b2-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="479b2-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="479b2-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="479b2-141">Content-Type</span></span>   | <span data-ttu-id="479b2-142">application/json</span><span class="sxs-lookup"><span data-stu-id="479b2-142">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="479b2-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="479b2-143">Request body</span></span>
<span data-ttu-id="479b2-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="479b2-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="479b2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="479b2-145">Response</span></span>

<span data-ttu-id="479b2-146">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="479b2-146">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="479b2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="479b2-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="479b2-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="479b2-148">Request</span></span>
<span data-ttu-id="479b2-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="479b2-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="479b2-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="479b2-150">Response</span></span>
<span data-ttu-id="479b2-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="479b2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
