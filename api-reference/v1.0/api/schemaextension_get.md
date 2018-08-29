# <a name="get-schemaextension"></a><span data-ttu-id="bffb6-101">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="bffb6-101">Get schemaExtension</span></span>
<span data-ttu-id="bffb6-102">Получение свойств указанного определения [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="bffb6-102">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="bffb6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bffb6-103">Permissions</span></span>
<span data-ttu-id="bffb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bffb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bffb6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bffb6-106">Permission type</span></span>      | <span data-ttu-id="bffb6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bffb6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bffb6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bffb6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bffb6-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bffb6-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bffb6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bffb6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bffb6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffb6-111">Not supported.</span></span>    |
|<span data-ttu-id="bffb6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bffb6-112">Application</span></span> | <span data-ttu-id="bffb6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffb6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bffb6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bffb6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bffb6-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bffb6-115">Optional query parameters</span></span>
<span data-ttu-id="bffb6-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bffb6-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bffb6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bffb6-117">Request headers</span></span>
| <span data-ttu-id="bffb6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bffb6-118">Name</span></span>      |<span data-ttu-id="bffb6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bffb6-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bffb6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bffb6-120">Authorization</span></span>  | <span data-ttu-id="bffb6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bffb6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bffb6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bffb6-123">Content-Type</span></span>   | <span data-ttu-id="bffb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bffb6-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bffb6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bffb6-125">Request body</span></span>
<span data-ttu-id="bffb6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bffb6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bffb6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bffb6-127">Response</span></span>

<span data-ttu-id="bffb6-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bffb6-128">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bffb6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bffb6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bffb6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bffb6-130">Request</span></span>
<span data-ttu-id="bffb6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bffb6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="bffb6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bffb6-132">Response</span></span>
<span data-ttu-id="bffb6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bffb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="bffb6-136">См. также</span><span class="sxs-lookup"><span data-stu-id="bffb6-136">See also</span></span>

- [<span data-ttu-id="bffb6-137">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="bffb6-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="bffb6-138">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="bffb6-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->