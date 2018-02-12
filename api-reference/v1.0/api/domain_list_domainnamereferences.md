# <a name="list-domainnamereferences"></a><span data-ttu-id="704d5-101">Перечисление domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="704d5-101">List domainNameReferences</span></span>

<span data-ttu-id="704d5-p101">Получение списка объектов [directoryObject](../resources/directoryobject.md) со ссылкой на домен. Возвращаемый список содержит все объекты каталога, у которых есть зависимости от домена.</span><span class="sxs-lookup"><span data-stu-id="704d5-p101">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="704d5-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="704d5-104">Permissions</span></span>

<span data-ttu-id="704d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="704d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="704d5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="704d5-107">Permission type</span></span>      | <span data-ttu-id="704d5-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="704d5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="704d5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="704d5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="704d5-110">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="704d5-110">Directory.Read.All</span></span>    |
|<span data-ttu-id="704d5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="704d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="704d5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="704d5-112">Not supported.</span></span>    |
|<span data-ttu-id="704d5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="704d5-113">Application</span></span> | <span data-ttu-id="704d5-114">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="704d5-114">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="704d5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="704d5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="704d5-116">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="704d5-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="704d5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="704d5-117">Optional query parameters</span></span>

<span data-ttu-id="704d5-118">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="704d5-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="704d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="704d5-119">Request headers</span></span>

| <span data-ttu-id="704d5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="704d5-120">Name</span></span>      |<span data-ttu-id="704d5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="704d5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="704d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="704d5-122">Authorization</span></span>  | <span data-ttu-id="704d5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="704d5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="704d5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="704d5-125">Request body</span></span>

<span data-ttu-id="704d5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="704d5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="704d5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="704d5-127">Response</span></span>

<span data-ttu-id="704d5-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="704d5-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="704d5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="704d5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="704d5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="704d5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="704d5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="704d5-131">Response</span></span>
<span data-ttu-id="704d5-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="704d5-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->