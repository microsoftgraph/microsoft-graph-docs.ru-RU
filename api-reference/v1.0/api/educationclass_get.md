# <a name="get-educationclass"></a><span data-ttu-id="c034e-101">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="c034e-101">Get educationClass</span></span>

<span data-ttu-id="c034e-102">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="c034e-102">Retrieve a class from the system.</span></span> <span data-ttu-id="c034e-103">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="c034e-103">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="c034e-104">Члены группы представляют учащихся, администраторы группы — преподавателей курса.</span><span class="sxs-lookup"><span data-stu-id="c034e-104">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="c034e-105">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="c034e-105">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="c034e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c034e-106">Permissions</span></span>
<span data-ttu-id="c034e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c034e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c034e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c034e-109">Permission type</span></span>      | <span data-ttu-id="c034e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c034e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c034e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c034e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c034e-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c034e-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c034e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c034e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c034e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c034e-114">Not supported</span></span>  |
|<span data-ttu-id="c034e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c034e-115">Application</span></span> | <span data-ttu-id="c034e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c034e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c034e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c034e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c034e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c034e-118">Optional query parameters</span></span>
<span data-ttu-id="c034e-119">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c034e-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c034e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c034e-120">Request headers</span></span>
| <span data-ttu-id="c034e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c034e-121">Header</span></span>       | <span data-ttu-id="c034e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c034e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c034e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c034e-123">Authorization</span></span>  | <span data-ttu-id="c034e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c034e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c034e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c034e-126">Request body</span></span>
<span data-ttu-id="c034e-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c034e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c034e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c034e-128">Response</span></span>
<span data-ttu-id="c034e-129">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c034e-129">If successful, this method returns a `200 OK` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c034e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c034e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c034e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c034e-131">Request</span></span>
<span data-ttu-id="c034e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c034e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="c034e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c034e-133">Response</span></span>
<span data-ttu-id="c034e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c034e-134">The following is an example of the response.</span></span> 

><span data-ttu-id="c034e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c034e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->