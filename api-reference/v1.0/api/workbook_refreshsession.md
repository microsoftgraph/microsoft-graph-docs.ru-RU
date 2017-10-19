# <a name="refresh-session"></a><span data-ttu-id="fa6dc-101">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="fa6dc-101">Refresh Session</span></span>

<span data-ttu-id="fa6dc-102">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-102">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fa6dc-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa6dc-103">Permissions</span></span>
<span data-ttu-id="fa6dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa6dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa6dc-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa6dc-106">Permission type</span></span>      | <span data-ttu-id="fa6dc-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa6dc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa6dc-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa6dc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fa6dc-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa6dc-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa6dc-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa6dc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa6dc-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-111">Not supported.</span></span>    |
|<span data-ttu-id="fa6dc-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa6dc-112">Application</span></span> | <span data-ttu-id="fa6dc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa6dc-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa6dc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="fa6dc-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa6dc-115">Request headers</span></span>
| <span data-ttu-id="fa6dc-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fa6dc-116">Name</span></span>       | <span data-ttu-id="fa6dc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fa6dc-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa6dc-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa6dc-118">Authorization</span></span>  | <span data-ttu-id="fa6dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa6dc-121">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="fa6dc-121">Workbook-Session-Id</span></span> | <span data-ttu-id="fa6dc-122">Идентификатор сеанса книги, который необходимо обновить</span><span class="sxs-lookup"><span data-stu-id="fa6dc-122">Workbook session Id to be refreshd</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa6dc-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa6dc-123">Request body</span></span>
<span data-ttu-id="fa6dc-124">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="fa6dc-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa6dc-125">Response</span></span>

<span data-ttu-id="fa6dc-126">В случае успешного выполнения этот метод возвращает код отклика `204, No content`.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-126">If successful, this method returns `204, No content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa6dc-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fa6dc-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa6dc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa6dc-128">Request</span></span>
<span data-ttu-id="fa6dc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

```

<span data-ttu-id="fa6dc-130">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="fa6dc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa6dc-131">Response</span></span>
<span data-ttu-id="fa6dc-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fa6dc-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```