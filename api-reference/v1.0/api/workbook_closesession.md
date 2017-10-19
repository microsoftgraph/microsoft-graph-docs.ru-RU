# <a name="close-session"></a><span data-ttu-id="7fb1f-101">Close Session</span><span class="sxs-lookup"><span data-stu-id="7fb1f-101">Close Session</span></span>

<span data-ttu-id="7fb1f-102">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-102">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7fb1f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb1f-103">Permissions</span></span>
<span data-ttu-id="7fb1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fb1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7fb1f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb1f-106">Permission type</span></span>      | <span data-ttu-id="7fb1f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fb1f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb1f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fb1f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7fb1f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fb1f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fb1f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fb1f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fb1f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-111">Not supported.</span></span>    |
|<span data-ttu-id="7fb1f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fb1f-112">Application</span></span> | <span data-ttu-id="7fb1f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fb1f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fb1f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="7fb1f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fb1f-115">Request headers</span></span>
| <span data-ttu-id="7fb1f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="7fb1f-116">Name</span></span>       | <span data-ttu-id="7fb1f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7fb1f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fb1f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fb1f-118">Authorization</span></span>  | <span data-ttu-id="7fb1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fb1f-121">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="7fb1f-121">Workbook-Session-Id</span></span> | <span data-ttu-id="7fb1f-122">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="7fb1f-122">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fb1f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fb1f-123">Request body</span></span>
<span data-ttu-id="7fb1f-124">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="7fb1f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb1f-125">Response</span></span>

<span data-ttu-id="7fb1f-126">В случае успешного выполнения этот метод возвращает код отклика `204, No content`.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-126">If successful, this method returns `204, No content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7fb1f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7fb1f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fb1f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fb1f-128">Request</span></span>
<span data-ttu-id="7fb1f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

```

<span data-ttu-id="7fb1f-130">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="7fb1f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb1f-131">Response</span></span>
<span data-ttu-id="7fb1f-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7fb1f-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```