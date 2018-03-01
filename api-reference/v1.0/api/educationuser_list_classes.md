# <a name="list-classes"></a><span data-ttu-id="78dc4-101">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="78dc4-101">List classes</span></span>

<span data-ttu-id="78dc4-102">Получение списка объектов курсов.</span><span class="sxs-lookup"><span data-stu-id="78dc4-102">Retrieve a list of chartpoints objects.</span></span> <span data-ttu-id="78dc4-103">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="78dc4-103">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="78dc4-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78dc4-104">Permissions</span></span>
<span data-ttu-id="78dc4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78dc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78dc4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78dc4-107">Permission type</span></span>      | <span data-ttu-id="78dc4-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78dc4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78dc4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78dc4-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="78dc4-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="78dc4-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="78dc4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78dc4-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="78dc4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78dc4-112">Not supported.</span></span>  |
|<span data-ttu-id="78dc4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78dc4-113">Application</span></span> | <span data-ttu-id="78dc4-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78dc4-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="78dc4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78dc4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78dc4-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78dc4-116">Optional query parameters</span></span>
<span data-ttu-id="78dc4-117">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="78dc4-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78dc4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78dc4-118">Request headers</span></span>
| <span data-ttu-id="78dc4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78dc4-119">Header</span></span>       | <span data-ttu-id="78dc4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="78dc4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78dc4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78dc4-121">Authorization</span></span>  | <span data-ttu-id="78dc4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78dc4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78dc4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78dc4-124">Request body</span></span>
<span data-ttu-id="78dc4-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78dc4-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78dc4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="78dc4-126">Response</span></span>
<span data-ttu-id="78dc4-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78dc4-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78dc4-128">Пример</span><span class="sxs-lookup"><span data-stu-id="78dc4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78dc4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="78dc4-129">Request</span></span>
<span data-ttu-id="78dc4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78dc4-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="78dc4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="78dc4-131">Response</span></span>
<span data-ttu-id="78dc4-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="78dc4-132">The following is an example of the response.</span></span> 

><span data-ttu-id="78dc4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78dc4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->