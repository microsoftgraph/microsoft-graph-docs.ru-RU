# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="aab81-101">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="aab81-101">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="aab81-102">Получение списка поддерживаемых языковых стандартов и языков, которые настроены на сервере почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="aab81-102">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="aab81-103">Настраивая клиент Outlook, пользователь выбирает язык из этого списка.</span><span class="sxs-lookup"><span data-stu-id="aab81-103">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="aab81-104">После этого вы можете получить выбранный язык вместе с [ настройками почтового ящика пользователя](user_get_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="aab81-104">You can subsequently get the preferred language by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="aab81-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aab81-105">Permissions</span></span>
<span data-ttu-id="aab81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aab81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aab81-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aab81-108">Permission type</span></span>      | <span data-ttu-id="aab81-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aab81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aab81-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aab81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aab81-111">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="aab81-111">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="aab81-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aab81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aab81-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="aab81-113">User.Read</span></span>    |
|<span data-ttu-id="aab81-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aab81-114">Application</span></span> | <span data-ttu-id="aab81-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="aab81-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aab81-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aab81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="aab81-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aab81-117">Request headers</span></span>
| <span data-ttu-id="aab81-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aab81-118">Name</span></span>       | <span data-ttu-id="aab81-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aab81-119">Type</span></span> | <span data-ttu-id="aab81-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aab81-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aab81-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab81-121">Authorization</span></span>  | <span data-ttu-id="aab81-122">string</span><span class="sxs-lookup"><span data-stu-id="aab81-122">string</span></span>  | <span data-ttu-id="aab81-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aab81-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="aab81-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aab81-125">Request body</span></span>
<span data-ttu-id="aab81-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aab81-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aab81-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="aab81-127">Response</span></span>
<span data-ttu-id="aab81-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [localeInfo](../resources/localeinfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aab81-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab81-129">Пример</span><span class="sxs-lookup"><span data-stu-id="aab81-129">Example</span></span>
<span data-ttu-id="aab81-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="aab81-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aab81-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aab81-131">Request</span></span>
<span data-ttu-id="aab81-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aab81-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="aab81-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aab81-133">Response</span></span>
<span data-ttu-id="aab81-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aab81-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->