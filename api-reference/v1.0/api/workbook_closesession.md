# <a name="close-session"></a><span data-ttu-id="70970-101">Close Session</span><span class="sxs-lookup"><span data-stu-id="70970-101">Close Session</span></span>

<span data-ttu-id="70970-102">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="70970-102">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="70970-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70970-103">Permissions</span></span>
<span data-ttu-id="70970-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="70970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70970-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70970-106">Permission type</span></span>      | <span data-ttu-id="70970-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70970-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70970-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70970-108">Delegated (work or school account)</span></span> | <span data-ttu-id="70970-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70970-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70970-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70970-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70970-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70970-111">Not supported.</span></span>    |
|<span data-ttu-id="70970-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70970-112">Application</span></span> | <span data-ttu-id="70970-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70970-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70970-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70970-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="70970-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70970-115">Request headers</span></span>
| <span data-ttu-id="70970-116">Имя</span><span class="sxs-lookup"><span data-stu-id="70970-116">Name</span></span>       | <span data-ttu-id="70970-117">Описание</span><span class="sxs-lookup"><span data-stu-id="70970-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70970-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70970-118">Authorization</span></span>  | <span data-ttu-id="70970-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70970-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="70970-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="70970-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="70970-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="70970-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="70970-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="70970-124">workbook-session-id</span></span> | <span data-ttu-id="70970-125">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="70970-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="70970-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70970-126">Request body</span></span>
<span data-ttu-id="70970-127">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="70970-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="70970-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="70970-128">Response</span></span>

<span data-ttu-id="70970-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70970-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70970-130">Пример</span><span class="sxs-lookup"><span data-stu-id="70970-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70970-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="70970-131">Request</span></span>
<span data-ttu-id="70970-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70970-132">Here is an example of the request.</span></span>
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

<span data-ttu-id="70970-133">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="70970-133">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="70970-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="70970-134">Response</span></span>
<span data-ttu-id="70970-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70970-135">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook_closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->