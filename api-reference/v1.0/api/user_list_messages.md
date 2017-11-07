# <a name="list-messages"></a><span data-ttu-id="23e7b-101">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="23e7b-101">List messages</span></span>

<span data-ttu-id="23e7b-102">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="23e7b-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="23e7b-103">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="23e7b-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="23e7b-104">Получение сообщений из папки другого пользователя</span><span class="sxs-lookup"><span data-stu-id="23e7b-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="23e7b-105">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить сообщения из папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="23e7b-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="23e7b-106">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="23e7b-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="23e7b-107">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="23e7b-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="23e7b-108">Предположим, что другой пользователь (Garth) поделился своей папкой сообщений с Никитой.</span><span class="sxs-lookup"><span data-stu-id="23e7b-108">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="23e7b-109">Вы можете получить сообщения из этой общей папки, указав идентификатор пользователя (или имя участника-пользователя) Garth, пример соответствующего запроса показан ниже.</span><span class="sxs-lookup"><span data-stu-id="23e7b-109">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="23e7b-110">Эта возможность распространяется на все поддерживаемые операции GET над сообщениями для отдельного пользователя, как показано в приведенном ниже разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="23e7b-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="23e7b-111">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="23e7b-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="23e7b-112">Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="23e7b-112">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="23e7b-113">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно получить сообщения только из папки пользователя, выполнившего вход, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="23e7b-113">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="23e7b-114">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="23e7b-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="23e7b-115">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="23e7b-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="23e7b-116">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="23e7b-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="23e7b-117">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="23e7b-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="23e7b-118">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="23e7b-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="23e7b-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23e7b-119">Permissions</span></span>
<span data-ttu-id="23e7b-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23e7b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23e7b-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23e7b-122">Permission type</span></span>      | <span data-ttu-id="23e7b-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23e7b-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23e7b-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23e7b-124">Delegated (work or school account)</span></span> | <span data-ttu-id="23e7b-125">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23e7b-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23e7b-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23e7b-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23e7b-127">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23e7b-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23e7b-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23e7b-128">Application</span></span> | <span data-ttu-id="23e7b-129">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23e7b-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23e7b-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23e7b-130">HTTP request</span></span>

<span data-ttu-id="23e7b-131">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="23e7b-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="23e7b-132">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="23e7b-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23e7b-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23e7b-133">Optional query parameters</span></span>
<span data-ttu-id="23e7b-134">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23e7b-134">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23e7b-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23e7b-135">Request headers</span></span>
| <span data-ttu-id="23e7b-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23e7b-136">Header</span></span>       | <span data-ttu-id="23e7b-137">Значение</span><span class="sxs-lookup"><span data-stu-id="23e7b-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23e7b-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23e7b-138">Authorization</span></span>  | <span data-ttu-id="23e7b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23e7b-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23e7b-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23e7b-141">Request body</span></span>
<span data-ttu-id="23e7b-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23e7b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e7b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="23e7b-143">Response</span></span>

<span data-ttu-id="23e7b-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23e7b-144">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="23e7b-145">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="23e7b-145">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="23e7b-146">Пример</span><span class="sxs-lookup"><span data-stu-id="23e7b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23e7b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="23e7b-147">Request</span></span>
<span data-ttu-id="23e7b-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23e7b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="23e7b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="23e7b-149">Response</span></span>
<span data-ttu-id="23e7b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23e7b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
