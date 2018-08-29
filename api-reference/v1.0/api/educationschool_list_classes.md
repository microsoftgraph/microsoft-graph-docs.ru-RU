# <a name="list-educationclasses"></a><span data-ttu-id="7f6e6-101">Перечисление educationClasses</span><span class="sxs-lookup"><span data-stu-id="7f6e6-101">List educationClasses</span></span>

<span data-ttu-id="7f6e6-102">Получение списка курсов учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-102">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f6e6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f6e6-103">Permissions</span></span>
<span data-ttu-id="7f6e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f6e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f6e6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f6e6-106">Permission type</span></span>      | <span data-ttu-id="7f6e6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f6e6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f6e6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f6e6-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f6e6-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="7f6e6-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="7f6e6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f6e6-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f6e6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-111">Not supported.</span></span>  |
|<span data-ttu-id="7f6e6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f6e6-112">Application</span></span> | <span data-ttu-id="7f6e6-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f6e6-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f6e6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f6e6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f6e6-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f6e6-115">Optional query parameters</span></span>
<span data-ttu-id="7f6e6-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f6e6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f6e6-117">Request headers</span></span>
| <span data-ttu-id="7f6e6-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f6e6-118">Header</span></span>       | <span data-ttu-id="7f6e6-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7f6e6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f6e6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f6e6-120">Authorization</span></span>  | <span data-ttu-id="7f6e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f6e6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f6e6-123">Request body</span></span>
<span data-ttu-id="7f6e6-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f6e6-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f6e6-125">Response</span></span>
<span data-ttu-id="7f6e6-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-126">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f6e6-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7f6e6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f6e6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f6e6-128">Request</span></span>
<span data-ttu-id="7f6e6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
##### <a name="response"></a><span data-ttu-id="7f6e6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f6e6-130">Response</span></span>
<span data-ttu-id="7f6e6-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-131">The following is an example of the response.</span></span> 

><span data-ttu-id="7f6e6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f6e6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
