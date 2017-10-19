# <a name="get-contactfolder"></a><span data-ttu-id="4b10c-101">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="4b10c-101">Get contactFolder</span></span>

<span data-ttu-id="4b10c-102">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="4b10c-102">Get a contact folder by using the contact folder ID.</span></span>


### <a name="get-another-users-contact-folder"></a><span data-ttu-id="4b10c-103">Получение папки контактов другого пользователя</span><span class="sxs-lookup"><span data-stu-id="4b10c-103">Get another user's contact folder</span></span>

<span data-ttu-id="4b10c-104">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить папку контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b10c-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="4b10c-105">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="4b10c-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="4b10c-106">Например, ваше приложение получило делегированные разрешения от пользователя John.</span><span class="sxs-lookup"><span data-stu-id="4b10c-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="4b10c-107">Предположим, что другой пользователь (Garth) поделился своей папкой контактов с пользователем John.</span><span class="sxs-lookup"><span data-stu-id="4b10c-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="4b10c-108">Вы можете получить эту общую папку, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="4b10c-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contactFolders/{id}
```

<span data-ttu-id="4b10c-109">Эта возможность применяется для всех операций GET над папкой контактов для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="4b10c-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="4b10c-110">Она также применяется, если пользователь Garth делегировал весь свой почтовый ящик пользователю John.</span><span class="sxs-lookup"><span data-stu-id="4b10c-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="4b10c-111">Если пользователь Garth не поделился своей папкой контактов с пользователем John и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="4b10c-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="4b10c-112">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить папку контактов пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="4b10c-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
```

<span data-ttu-id="4b10c-113">Эта возможность доступна только в операциях GET для:</span><span class="sxs-lookup"><span data-stu-id="4b10c-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="4b10c-114">общих папок контактов;</span><span class="sxs-lookup"><span data-stu-id="4b10c-114">Shared contact folders</span></span>
- <span data-ttu-id="4b10c-115">общих календарей;</span><span class="sxs-lookup"><span data-stu-id="4b10c-115">Shared calendars</span></span>
- <span data-ttu-id="4b10c-116">контактов и событий в общих папках;</span><span class="sxs-lookup"><span data-stu-id="4b10c-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="4b10c-117">указанных выше ресурсов в делегированных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="4b10c-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="4b10c-118">Эта возможность недоступна в других операциях для контактов, событий и их папок.</span><span class="sxs-lookup"><span data-stu-id="4b10c-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="4b10c-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b10c-119">Permissions</span></span>
<span data-ttu-id="4b10c-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b10c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b10c-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b10c-122">Permission type</span></span>      | <span data-ttu-id="4b10c-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b10c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b10c-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b10c-124">Delegated (work or school account)</span></span> | <span data-ttu-id="4b10c-125">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b10c-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4b10c-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b10c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b10c-127">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b10c-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4b10c-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b10c-128">Application</span></span> | <span data-ttu-id="4b10c-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b10c-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b10c-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b10c-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b10c-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b10c-131">Optional query parameters</span></span>
<span data-ttu-id="4b10c-132">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b10c-132">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b10c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b10c-133">Request headers</span></span>
| <span data-ttu-id="4b10c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="4b10c-134">Name</span></span>       | <span data-ttu-id="4b10c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4b10c-135">Type</span></span> | <span data-ttu-id="4b10c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4b10c-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b10c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b10c-137">Authorization</span></span>  | <span data-ttu-id="4b10c-138">string</span><span class="sxs-lookup"><span data-stu-id="4b10c-138">string</span></span>  | <span data-ttu-id="4b10c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b10c-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b10c-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b10c-141">Request body</span></span>
<span data-ttu-id="4b10c-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b10c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b10c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b10c-143">Response</span></span>

<span data-ttu-id="4b10c-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b10c-144">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b10c-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4b10c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b10c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b10c-146">Request</span></span>
<span data-ttu-id="4b10c-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b10c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="4b10c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b10c-148">Response</span></span>
<span data-ttu-id="4b10c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b10c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
