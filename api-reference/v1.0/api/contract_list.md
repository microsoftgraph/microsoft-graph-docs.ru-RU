# <a name="list-contracts"></a><span data-ttu-id="c548c-101">Перечисление contract</span><span class="sxs-lookup"><span data-stu-id="c548c-101">List contracts</span></span>

<span data-ttu-id="c548c-102">Получение списка объектов [contract](../resources/contract.md), сопоставленных с клиентом партнера.</span><span class="sxs-lookup"><span data-stu-id="c548c-102">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c548c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c548c-103">Permissions</span></span>

<span data-ttu-id="c548c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c548c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c548c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c548c-106">Permission type</span></span>      | <span data-ttu-id="c548c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c548c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c548c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c548c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c548c-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c548c-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="c548c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c548c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c548c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c548c-111">Not supported.</span></span>    | 
|<span data-ttu-id="c548c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c548c-112">Application</span></span> | <span data-ttu-id="c548c-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c548c-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c548c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c548c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c548c-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c548c-115">Optional query parameters</span></span>

<span data-ttu-id="c548c-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c548c-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="c548c-117">Для свойств customerId, defaultDomainName и displayName поддерживается фильтрация.</span><span class="sxs-lookup"><span data-stu-id="c548c-117">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c548c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c548c-118">Request headers</span></span>

| <span data-ttu-id="c548c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c548c-119">Name</span></span>      |<span data-ttu-id="c548c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c548c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c548c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c548c-121">Authorization</span></span>  | <span data-ttu-id="c548c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c548c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c548c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c548c-124">Request body</span></span>

<span data-ttu-id="c548c-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c548c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c548c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c548c-126">Response</span></span>

<span data-ttu-id="c548c-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c548c-127">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c548c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c548c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c548c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c548c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="c548c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c548c-130">Response</span></span>

<span data-ttu-id="c548c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c548c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->