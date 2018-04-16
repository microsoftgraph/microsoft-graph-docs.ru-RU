# <a name="create-outlook-category"></a><span data-ttu-id="3c938-101">Создание категории Outlook</span><span class="sxs-lookup"><span data-stu-id="3c938-101">Create Outlook category</span></span>


<span data-ttu-id="3c938-102">Создание объекта [outlookCategory](../resources/outlookCategory.md) в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c938-102">Create an [outlookCategory](../resources/outlookCategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c938-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c938-103">Permissions</span></span>
<span data-ttu-id="3c938-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c938-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c938-106">Permission type</span></span>      | <span data-ttu-id="3c938-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c938-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c938-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c938-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3c938-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c938-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3c938-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c938-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c938-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c938-111">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="3c938-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c938-112">Application</span></span> | <span data-ttu-id="3c938-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c938-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c938-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c938-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="3c938-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c938-115">Request headers</span></span>
| <span data-ttu-id="3c938-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3c938-116">Name</span></span>       | <span data-ttu-id="3c938-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3c938-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3c938-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c938-118">Authorization</span></span>  | <span data-ttu-id="3c938-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c938-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3c938-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c938-121">Request body</span></span>
<span data-ttu-id="3c938-122">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookCategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c938-122">In the request body, supply a JSON representation of [plannerTask](../resources/outlookCategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c938-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c938-123">Response</span></span>

<span data-ttu-id="3c938-124">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [outlookCategory](../resources/outlookCategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c938-124">If successful, this method returns `201 Created` response code and the new [page](../resources/outlookCategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c938-125">Пример</span><span class="sxs-lookup"><span data-stu-id="3c938-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c938-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c938-126">Request</span></span>
<span data-ttu-id="3c938-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c938-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="3c938-128">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookCategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c938-128">In the request body, supply a JSON representation of [plannerTask](../resources/outlookCategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3c938-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c938-129">Response</span></span>
<span data-ttu-id="3c938-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c938-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->