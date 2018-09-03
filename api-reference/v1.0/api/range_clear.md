# <a name="range-clear"></a><span data-ttu-id="c705c-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="c705c-101">Range: clear</span></span>

<span data-ttu-id="c705c-102">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="c705c-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="c705c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c705c-103">Permissions</span></span>
<span data-ttu-id="c705c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c705c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c705c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c705c-106">Permission type</span></span>      | <span data-ttu-id="c705c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c705c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c705c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c705c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c705c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c705c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c705c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c705c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c705c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c705c-111">Not supported.</span></span>    |
|<span data-ttu-id="c705c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c705c-112">Application</span></span> | <span data-ttu-id="c705c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c705c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c705c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c705c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="c705c-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c705c-115">Request headers</span></span>
| <span data-ttu-id="c705c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c705c-116">Name</span></span>       | <span data-ttu-id="c705c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c705c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c705c-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c705c-118">Authorization</span></span>  | <span data-ttu-id="c705c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c705c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c705c-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c705c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c705c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c705c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c705c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c705c-124">Request body</span></span>
<span data-ttu-id="c705c-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c705c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c705c-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="c705c-126">Parameter</span></span>    | <span data-ttu-id="c705c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c705c-127">Type</span></span>   |<span data-ttu-id="c705c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c705c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c705c-129">applyTo</span><span class="sxs-lookup"><span data-stu-id="c705c-129">applyTo</span></span>|<span data-ttu-id="c705c-130">string (строка)</span><span class="sxs-lookup"><span data-stu-id="c705c-130">string</span></span>|<span data-ttu-id="c705c-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c705c-131">Optional.</span></span> <span data-ttu-id="c705c-132">Определяет тип действия очистки.</span><span class="sxs-lookup"><span data-stu-id="c705c-132">Optional. Determines the type of clear action.  Possible values are: , , .</span></span>  <span data-ttu-id="c705c-133">Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="c705c-133">The possible values are `All`, `Formats`, `Contents`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="c705c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c705c-134">Response</span></span>

<span data-ttu-id="c705c-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c705c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c705c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c705c-137">Example</span></span>
<span data-ttu-id="c705c-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c705c-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c705c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c705c-139">Request</span></span>
<span data-ttu-id="c705c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c705c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="c705c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c705c-141">Response</span></span>
<span data-ttu-id="c705c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c705c-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->