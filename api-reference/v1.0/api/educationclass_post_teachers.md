# <a name="add-teacher"></a><span data-ttu-id="9a273-101">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="9a273-101">Add teacher</span></span>

<span data-ttu-id="9a273-102">Добавление преподавателя в класс.</span><span class="sxs-lookup"><span data-stu-id="9a273-102">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a273-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a273-103">Permissions</span></span>
<span data-ttu-id="9a273-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a273-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a273-106">Permission type</span></span>      | <span data-ttu-id="9a273-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a273-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a273-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a273-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9a273-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a273-109">Not supported.</span></span>  |
|<span data-ttu-id="9a273-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a273-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9a273-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a273-111">Not supported.</span></span>  |
|<span data-ttu-id="9a273-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a273-112">Application</span></span> | <span data-ttu-id="9a273-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a273-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9a273-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a273-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9a273-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a273-115">Request headers</span></span>
| <span data-ttu-id="9a273-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a273-116">Header</span></span>       | <span data-ttu-id="9a273-117">Значение</span><span class="sxs-lookup"><span data-stu-id="9a273-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a273-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a273-118">Authorization</span></span>  | <span data-ttu-id="9a273-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a273-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9a273-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a273-121">Content-Type</span></span>  | <span data-ttu-id="9a273-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9a273-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a273-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a273-123">Request body</span></span>
<span data-ttu-id="9a273-124">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a273-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9a273-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a273-125">Response</span></span>
<span data-ttu-id="9a273-126">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a273-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a273-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9a273-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a273-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a273-128">Request</span></span>
<span data-ttu-id="9a273-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a273-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="9a273-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a273-130">Response</span></span>
<span data-ttu-id="9a273-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a273-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="9a273-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a273-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
