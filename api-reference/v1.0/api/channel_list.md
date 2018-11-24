# <a name="list-channels"></a><span data-ttu-id="506d1-101">Список каналов</span><span class="sxs-lookup"><span data-stu-id="506d1-101">List channels</span></span>



<span data-ttu-id="506d1-102">Получить список [каналов](../resources/channel.md) из этой группы.</span><span class="sxs-lookup"><span data-stu-id="506d1-102">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="506d1-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="506d1-103">Permissions</span></span>
<span data-ttu-id="506d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="506d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="506d1-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="506d1-106">Permission type</span></span>      | <span data-ttu-id="506d1-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="506d1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="506d1-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="506d1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="506d1-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506d1-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="506d1-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="506d1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="506d1-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506d1-111">Not supported.</span></span>    |
|<span data-ttu-id="506d1-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="506d1-112">Application</span></span> | <span data-ttu-id="506d1-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506d1-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="506d1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="506d1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="506d1-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="506d1-115">Optional query parameters</span></span>
<span data-ttu-id="506d1-116">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="506d1-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="506d1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="506d1-117">Request headers</span></span>
| <span data-ttu-id="506d1-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="506d1-118">Header</span></span>       | <span data-ttu-id="506d1-119">Значение</span><span class="sxs-lookup"><span data-stu-id="506d1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="506d1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="506d1-120">Authorization</span></span>  | <span data-ttu-id="506d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="506d1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="506d1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="506d1-123">Request body</span></span>
<span data-ttu-id="506d1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="506d1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="506d1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="506d1-125">Response</span></span>

<span data-ttu-id="506d1-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="506d1-126">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506d1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="506d1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="506d1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="506d1-128">Request</span></span>
<span data-ttu-id="506d1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="506d1-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="506d1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="506d1-130">Response</span></span>
<span data-ttu-id="506d1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="506d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
