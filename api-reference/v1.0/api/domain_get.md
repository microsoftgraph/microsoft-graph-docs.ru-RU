# <a name="get-domain"></a><span data-ttu-id="26b77-101">Получение домена</span><span class="sxs-lookup"><span data-stu-id="26b77-101">Get domain</span></span>

<span data-ttu-id="26b77-102">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="26b77-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b77-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26b77-103">Permissions</span></span>

<span data-ttu-id="26b77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="26b77-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b77-106">Permission type</span></span>      | <span data-ttu-id="26b77-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b77-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26b77-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b77-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26b77-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b77-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="26b77-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b77-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b77-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b77-111">Not supported.</span></span>    |
|<span data-ttu-id="26b77-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b77-112">Application</span></span> | <span data-ttu-id="26b77-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b77-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26b77-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b77-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="26b77-115">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="26b77-115">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="26b77-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26b77-116">Optional query parameters</span></span>

<span data-ttu-id="26b77-117">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="26b77-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26b77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b77-118">Request headers</span></span>

| <span data-ttu-id="26b77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26b77-119">Name</span></span>      |<span data-ttu-id="26b77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26b77-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26b77-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b77-121">Authorization</span></span>  | <span data-ttu-id="26b77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26b77-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26b77-124">Content-Type</span></span>  | <span data-ttu-id="26b77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26b77-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b77-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26b77-126">Request body</span></span>
<span data-ttu-id="26b77-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26b77-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b77-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b77-128">Response</span></span>

<span data-ttu-id="26b77-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26b77-129">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26b77-130">Пример</span><span class="sxs-lookup"><span data-stu-id="26b77-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26b77-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b77-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="26b77-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b77-132">Response</span></span>
<span data-ttu-id="26b77-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26b77-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->