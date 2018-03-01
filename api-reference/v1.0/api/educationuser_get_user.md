# <a name="get-user"></a><span data-ttu-id="7389e-101">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="7389e-101">Get user</span></span>

<span data-ttu-id="7389e-102">Получение простого каталога **user**, который соответствует этому объекту **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="7389e-102">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="7389e-103">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="7389e-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="7389e-104">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="7389e-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7389e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7389e-105">Permissions</span></span>
<span data-ttu-id="7389e-106">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="7389e-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="7389e-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7389e-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7389e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7389e-108">Permission type</span></span>      | <span data-ttu-id="7389e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7389e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7389e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7389e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7389e-111">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All или User.Read</span><span class="sxs-lookup"><span data-stu-id="7389e-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="7389e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7389e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7389e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7389e-113">Not supported.</span></span>  |
|<span data-ttu-id="7389e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7389e-114">Application</span></span> | <span data-ttu-id="7389e-115">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7389e-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7389e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7389e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="7389e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7389e-117">Request headers</span></span>
| <span data-ttu-id="7389e-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7389e-118">Header</span></span>       | <span data-ttu-id="7389e-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7389e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7389e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7389e-120">Authorization</span></span>  | <span data-ttu-id="7389e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7389e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7389e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7389e-123">Request body</span></span>
<span data-ttu-id="7389e-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7389e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7389e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7389e-125">Response</span></span>
<span data-ttu-id="7389e-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7389e-126">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7389e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7389e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7389e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7389e-128">Request</span></span>
<span data-ttu-id="7389e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7389e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
##### <a name="response"></a><span data-ttu-id="7389e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7389e-130">Response</span></span>
<span data-ttu-id="7389e-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7389e-131">The following is an example of the response.</span></span> 

><span data-ttu-id="7389e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7389e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->