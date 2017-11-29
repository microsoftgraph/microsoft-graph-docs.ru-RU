# <a name="close-session"></a><span data-ttu-id="fb01b-101">Close Session</span><span class="sxs-lookup"><span data-stu-id="fb01b-101">Close Session</span></span>

<span data-ttu-id="fb01b-102">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="fb01b-102">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fb01b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb01b-103">Permissions</span></span>
<span data-ttu-id="fb01b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb01b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb01b-106">Permission type</span></span>      | <span data-ttu-id="fb01b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb01b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb01b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb01b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb01b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb01b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb01b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb01b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb01b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb01b-111">Not supported.</span></span>    |
|<span data-ttu-id="fb01b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb01b-112">Application</span></span> | <span data-ttu-id="fb01b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb01b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb01b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb01b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="fb01b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb01b-115">Request headers</span></span>
| <span data-ttu-id="fb01b-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fb01b-116">Name</span></span>       | <span data-ttu-id="fb01b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fb01b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb01b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb01b-118">Authorization</span></span>  | <span data-ttu-id="fb01b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb01b-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="fb01b-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb01b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb01b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fb01b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="fb01b-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="fb01b-124">workbook-session-id</span></span> | <span data-ttu-id="fb01b-125">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="fb01b-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb01b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb01b-126">Request body</span></span>
<span data-ttu-id="fb01b-127">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="fb01b-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="fb01b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb01b-128">Response</span></span>

<span data-ttu-id="fb01b-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb01b-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb01b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb01b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb01b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb01b-131">Request</span></span>
<span data-ttu-id="fb01b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb01b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="fb01b-133">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="fb01b-133">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="fb01b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb01b-134">Response</span></span>
<span data-ttu-id="fb01b-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fb01b-135">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```