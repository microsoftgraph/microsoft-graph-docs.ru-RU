# <a name="refresh-session"></a><span data-ttu-id="e8391-101">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="e8391-101">Refresh Session</span></span>

<span data-ttu-id="e8391-102">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="e8391-102">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e8391-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8391-103">Permissions</span></span>
<span data-ttu-id="e8391-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8391-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8391-106">Permission type</span></span>      | <span data-ttu-id="e8391-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8391-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8391-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8391-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e8391-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8391-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8391-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8391-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8391-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8391-111">Not supported.</span></span>    |
|<span data-ttu-id="e8391-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8391-112">Application</span></span> | <span data-ttu-id="e8391-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8391-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8391-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8391-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="e8391-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8391-115">Request headers</span></span>
| <span data-ttu-id="e8391-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e8391-116">Name</span></span>       | <span data-ttu-id="e8391-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e8391-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8391-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8391-118">Authorization</span></span>  | <span data-ttu-id="e8391-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8391-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8391-121">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="e8391-121">workbook-session-id</span></span> | <span data-ttu-id="e8391-122">Идентификатор сеанса книги, который необходимо обновить</span><span class="sxs-lookup"><span data-stu-id="e8391-122">Workbook session Id to be refreshd</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8391-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8391-123">Request body</span></span>
<span data-ttu-id="e8391-124">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="e8391-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="e8391-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8391-125">Response</span></span>

<span data-ttu-id="e8391-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8391-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8391-127">Пример</span><span class="sxs-lookup"><span data-stu-id="e8391-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8391-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8391-128">Request</span></span>
<span data-ttu-id="e8391-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8391-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="e8391-130">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e8391-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="e8391-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8391-131">Response</span></span>
<span data-ttu-id="e8391-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8391-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```