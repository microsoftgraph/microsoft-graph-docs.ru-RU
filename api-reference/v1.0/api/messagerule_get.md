# <a name="get-rule"></a><span data-ttu-id="0d2e6-101">Получение правила</span><span class="sxs-lookup"><span data-stu-id="0d2e6-101">Get rule</span></span>


<span data-ttu-id="0d2e6-102">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="0d2e6-102">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="0d2e6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2e6-103">Permissions</span></span>
<span data-ttu-id="0d2e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d2e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d2e6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2e6-106">Permission type</span></span>      | <span data-ttu-id="0d2e6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d2e6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2e6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d2e6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2e6-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0d2e6-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0d2e6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d2e6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2e6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0d2e6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0d2e6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d2e6-112">Application</span></span> | <span data-ttu-id="0d2e6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0d2e6-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2e6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d2e6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d2e6-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0d2e6-115">Optional query parameters</span></span>
<span data-ttu-id="0d2e6-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d2e6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d2e6-117">Request headers</span></span>
| <span data-ttu-id="0d2e6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0d2e6-118">Name</span></span>      |<span data-ttu-id="0d2e6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2e6-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d2e6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d2e6-120">Authorization</span></span>  | <span data-ttu-id="0d2e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0d2e6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d2e6-123">Request body</span></span>
<span data-ttu-id="0d2e6-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0d2e6-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2e6-125">Response</span></span>
<span data-ttu-id="0d2e6-126">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-126">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d2e6-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0d2e6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d2e6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d2e6-128">Request</span></span>
<span data-ttu-id="0d2e6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="0d2e6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2e6-130">Response</span></span>
<span data-ttu-id="0d2e6-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-131">Here is an example of the response.</span></span> <span data-ttu-id="0d2e6-132">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-132">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="0d2e6-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d2e6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->