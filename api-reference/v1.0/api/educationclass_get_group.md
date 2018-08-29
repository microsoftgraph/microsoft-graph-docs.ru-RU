# <a name="get-group"></a><span data-ttu-id="18236-101">Получение группы</span><span class="sxs-lookup"><span data-stu-id="18236-101">Get group</span></span>

<span data-ttu-id="18236-102">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="18236-102">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="18236-103">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="18236-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="18236-104">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="18236-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="18236-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18236-105">Permissions</span></span>
<span data-ttu-id="18236-106">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="18236-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="18236-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18236-107">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18236-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18236-108">Permission type</span></span>      | <span data-ttu-id="18236-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18236-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18236-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18236-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="18236-111">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="18236-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="18236-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18236-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18236-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18236-113">Not supported.</span></span>  |
|<span data-ttu-id="18236-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18236-114">Application</span></span> | <span data-ttu-id="18236-115">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="18236-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="18236-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18236-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="18236-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18236-117">Request headers</span></span>
| <span data-ttu-id="18236-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18236-118">Header</span></span>       | <span data-ttu-id="18236-119">Значение</span><span class="sxs-lookup"><span data-stu-id="18236-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18236-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18236-120">Authorization</span></span>  | <span data-ttu-id="18236-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18236-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18236-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18236-123">Request body</span></span>
<span data-ttu-id="18236-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18236-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="18236-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="18236-125">Response</span></span>
<span data-ttu-id="18236-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18236-126">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18236-127">Пример</span><span class="sxs-lookup"><span data-stu-id="18236-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18236-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="18236-128">Request</span></span>
<span data-ttu-id="18236-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18236-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="18236-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="18236-130">Response</span></span>
<span data-ttu-id="18236-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18236-131">The following is an example of the response.</span></span> 

><span data-ttu-id="18236-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18236-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->