# <a name="get-contactfolder"></a><span data-ttu-id="29a35-101">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="29a35-101">Get contactFolder</span></span>

<span data-ttu-id="29a35-102">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="29a35-102">Get a contact folder by using the contact folder ID.</span></span>


### <a name="get-another-users-contact-folder"></a><span data-ttu-id="29a35-103">Получение папки контактов другого пользователя</span><span class="sxs-lookup"><span data-stu-id="29a35-103">Get another user's contact folder</span></span>

<span data-ttu-id="29a35-104">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить папку контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="29a35-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="29a35-105">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="29a35-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="29a35-106">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="29a35-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="29a35-107">Предположим, что другой пользователь (Garth) поделился своей папкой контактов с Никитой.</span><span class="sxs-lookup"><span data-stu-id="29a35-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="29a35-108">Вы можете получить эту общую папку, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="29a35-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contactFolders/{id}
```

<span data-ttu-id="29a35-109">Эта возможность применяется для всех операций GET над папкой контактов для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="29a35-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="29a35-110">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="29a35-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="29a35-111">Если пользователь Garth не поделился своей папкой контактов с Никитой и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="29a35-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="29a35-112">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить папку контактов пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="29a35-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
```

<span data-ttu-id="29a35-113">Эта возможность доступна только в операциях GET для:</span><span class="sxs-lookup"><span data-stu-id="29a35-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="29a35-114">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="29a35-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="29a35-115">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="29a35-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="29a35-116">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="29a35-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="29a35-117">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="29a35-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="29a35-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29a35-118">Permissions</span></span>
<span data-ttu-id="29a35-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29a35-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29a35-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29a35-121">Permission type</span></span>      | <span data-ttu-id="29a35-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29a35-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29a35-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29a35-123">Delegated (work or school account)</span></span> | <span data-ttu-id="29a35-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29a35-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="29a35-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29a35-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a35-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29a35-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="29a35-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29a35-127">Application</span></span> | <span data-ttu-id="29a35-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29a35-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="29a35-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29a35-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29a35-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29a35-130">Optional query parameters</span></span>
<span data-ttu-id="29a35-131">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="29a35-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29a35-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29a35-132">Request headers</span></span>
| <span data-ttu-id="29a35-133">Имя</span><span class="sxs-lookup"><span data-stu-id="29a35-133">Name</span></span>       | <span data-ttu-id="29a35-134">Тип</span><span class="sxs-lookup"><span data-stu-id="29a35-134">Type</span></span> | <span data-ttu-id="29a35-135">Описание</span><span class="sxs-lookup"><span data-stu-id="29a35-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29a35-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="29a35-136">Authorization</span></span>  | <span data-ttu-id="29a35-137">string</span><span class="sxs-lookup"><span data-stu-id="29a35-137">string</span></span>  | <span data-ttu-id="29a35-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29a35-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29a35-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29a35-140">Request body</span></span>
<span data-ttu-id="29a35-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29a35-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29a35-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="29a35-142">Response</span></span>

<span data-ttu-id="29a35-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29a35-143">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29a35-144">Пример</span><span class="sxs-lookup"><span data-stu-id="29a35-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29a35-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="29a35-145">Request</span></span>
<span data-ttu-id="29a35-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29a35-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="29a35-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="29a35-147">Response</span></span>
<span data-ttu-id="29a35-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="29a35-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
