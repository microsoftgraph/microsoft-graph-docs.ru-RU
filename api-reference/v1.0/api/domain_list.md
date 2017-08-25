# <a name="list-domains"></a><span data-ttu-id="b1365-101">Перечисление доменов</span><span class="sxs-lookup"><span data-stu-id="b1365-101">List domains</span></span>

<span data-ttu-id="b1365-102">Получение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="b1365-102">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1365-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1365-103">Permissions</span></span>
<span data-ttu-id="b1365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1365-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1365-106">Permission type</span></span>      | <span data-ttu-id="b1365-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1365-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b1365-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1365-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b1365-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1365-109">Directory.Read.All</span></span>    | 
|<span data-ttu-id="b1365-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1365-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1365-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1365-111">Not supported.</span></span>    | 
|<span data-ttu-id="b1365-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1365-112">Application</span></span> | <span data-ttu-id="b1365-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1365-113">Directory.Read.All, Domain.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1365-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1365-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1365-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1365-115">Optional query parameters</span></span>
<span data-ttu-id="b1365-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b1365-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1365-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1365-117">Request headers</span></span>
| <span data-ttu-id="b1365-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1365-118">Name</span></span>      |<span data-ttu-id="b1365-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b1365-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1365-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1365-120">Authorization</span></span>  | <span data-ttu-id="b1365-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1365-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b1365-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b1365-123">Accept</span></span>         | <span data-ttu-id="b1365-124">application/json;</span><span class="sxs-lookup"><span data-stu-id="b1365-124">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1365-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1365-125">Request body</span></span>
<span data-ttu-id="b1365-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1365-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1365-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1365-127">Response</span></span>

<span data-ttu-id="b1365-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1365-128">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1365-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b1365-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1365-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1365-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains
```
##### <a name="response"></a><span data-ttu-id="b1365-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1365-131">Response</span></span>
<span data-ttu-id="b1365-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1365-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->