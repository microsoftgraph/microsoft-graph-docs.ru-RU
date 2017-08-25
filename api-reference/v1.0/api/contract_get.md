# <a name="get-contract"></a><span data-ttu-id="9024d-101">Получение Contract</span><span class="sxs-lookup"><span data-stu-id="9024d-101">Get Contract</span></span>

<span data-ttu-id="9024d-102">Получение свойств и связей объекта [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="9024d-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9024d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9024d-103">Permissions</span></span>

<span data-ttu-id="9024d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9024d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9024d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9024d-106">Permission type</span></span>      | <span data-ttu-id="9024d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9024d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9024d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9024d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9024d-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9024d-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="9024d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9024d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9024d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9024d-111">Not supported.</span></span>    | 
|<span data-ttu-id="9024d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9024d-112">Application</span></span> | <span data-ttu-id="9024d-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9024d-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9024d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9024d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9024d-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9024d-115">Optional query parameters</span></span>

<span data-ttu-id="9024d-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9024d-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9024d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9024d-117">Request headers</span></span>

| <span data-ttu-id="9024d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9024d-118">Name</span></span>      |<span data-ttu-id="9024d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9024d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9024d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9024d-120">Authorization</span></span>  | <span data-ttu-id="9024d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9024d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9024d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9024d-123">Request body</span></span>

<span data-ttu-id="9024d-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9024d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9024d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9024d-125">Response</span></span>

<span data-ttu-id="9024d-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9024d-126">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9024d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9024d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9024d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9024d-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="9024d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9024d-129">Response</span></span>
<span data-ttu-id="9024d-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9024d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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