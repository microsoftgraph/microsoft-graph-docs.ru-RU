# <a name="get-mailfolder"></a><span data-ttu-id="757cc-101">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="757cc-101">Get mailFolder</span></span>

<span data-ttu-id="757cc-102">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="757cc-102">Retrieve the properties and relationships of a message object.</span></span>


### <a name="get-another-users-message-folder"></a><span data-ttu-id="757cc-103">Получение сообщений из папки другого пользователя</span><span class="sxs-lookup"><span data-stu-id="757cc-103">Get another user's contact folder</span></span>

<span data-ttu-id="757cc-104">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить папку сообщений, принадлежащую другому пользователю.</span><span class="sxs-lookup"><span data-stu-id="757cc-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="757cc-105">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="757cc-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="757cc-106">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="757cc-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="757cc-107">Предположим, что другой пользователь (Garth) поделился своей папкой сообщений с Никитой.</span><span class="sxs-lookup"><span data-stu-id="757cc-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="757cc-108">Вы можете получить эту общую папку, указав идентификатор пользователя (или имя участника-пользователя) Garth, пример соответствующего запроса показан ниже.</span><span class="sxs-lookup"><span data-stu-id="757cc-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

<span data-ttu-id="757cc-109">Эта возможность распространяется на все операции GET над папкой сообщений для отдельного пользователя, как показано в приведенном ниже разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="757cc-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="757cc-110">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="757cc-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="757cc-111">Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="757cc-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="757cc-112">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно получить только папку сообщений пользователя, выполнившего вход, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="757cc-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

<span data-ttu-id="757cc-113">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="757cc-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="757cc-114">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="757cc-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="757cc-115">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="757cc-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="757cc-116">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="757cc-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="757cc-117">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="757cc-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="757cc-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="757cc-118">Permissions</span></span>
<span data-ttu-id="757cc-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="757cc-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="757cc-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="757cc-121">Permission type</span></span>      | <span data-ttu-id="757cc-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="757cc-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="757cc-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="757cc-123">Delegated (work or school account)</span></span> | <span data-ttu-id="757cc-124">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="757cc-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="757cc-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="757cc-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="757cc-126">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="757cc-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="757cc-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="757cc-127">Application</span></span> | <span data-ttu-id="757cc-128">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="757cc-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="757cc-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="757cc-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="757cc-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="757cc-130">Optional query parameters</span></span>
<span data-ttu-id="757cc-131">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="757cc-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="757cc-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="757cc-132">Request headers</span></span>
| <span data-ttu-id="757cc-133">Имя</span><span class="sxs-lookup"><span data-stu-id="757cc-133">Name</span></span>       | <span data-ttu-id="757cc-134">Тип</span><span class="sxs-lookup"><span data-stu-id="757cc-134">Type</span></span> | <span data-ttu-id="757cc-135">Описание</span><span class="sxs-lookup"><span data-stu-id="757cc-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="757cc-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="757cc-136">Authorization</span></span>  | <span data-ttu-id="757cc-137">string</span><span class="sxs-lookup"><span data-stu-id="757cc-137">string</span></span>  | <span data-ttu-id="757cc-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="757cc-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="757cc-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="757cc-140">Request body</span></span>
<span data-ttu-id="757cc-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="757cc-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="757cc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="757cc-142">Response</span></span>

<span data-ttu-id="757cc-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="757cc-143">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="757cc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="757cc-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="757cc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="757cc-145">Request</span></span>
<span data-ttu-id="757cc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="757cc-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="757cc-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="757cc-147">Response</span></span>
<span data-ttu-id="757cc-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="757cc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
