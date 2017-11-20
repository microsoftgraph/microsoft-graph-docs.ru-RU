# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="4c775-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="4c775-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="4c775-102">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="4c775-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="4c775-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c775-103">Permissions</span></span>
<span data-ttu-id="4c775-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c775-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c775-106">Permission type</span></span>      | <span data-ttu-id="4c775-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c775-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c775-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c775-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4c775-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c775-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4c775-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c775-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c775-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c775-111">Not supported.</span></span>    |
|<span data-ttu-id="4c775-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c775-112">Application</span></span> | <span data-ttu-id="4c775-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c775-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c775-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c775-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="4c775-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c775-115">Request headers</span></span>
| <span data-ttu-id="4c775-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4c775-116">Name</span></span>       | <span data-ttu-id="4c775-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4c775-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c775-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c775-118">Authorization</span></span>  | <span data-ttu-id="4c775-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c775-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c775-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4c775-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4c775-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c775-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c775-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c775-124">Request body</span></span>
<span data-ttu-id="4c775-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4c775-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c775-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c775-126">Parameter</span></span>    | <span data-ttu-id="4c775-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4c775-127">Type</span></span>   |<span data-ttu-id="4c775-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4c775-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c775-129">password</span><span class="sxs-lookup"><span data-stu-id="4c775-129">password</span></span>|<span data-ttu-id="4c775-130">string</span><span class="sxs-lookup"><span data-stu-id="4c775-130">string</span></span>|<span data-ttu-id="4c775-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="4c775-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="4c775-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c775-133">Response</span></span>

<span data-ttu-id="4c775-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c775-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c775-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4c775-136">Example</span></span>
<span data-ttu-id="4c775-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4c775-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4c775-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c775-138">Request</span></span>
<span data-ttu-id="4c775-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c775-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="4c775-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c775-140">Response</span></span>
<span data-ttu-id="4c775-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c775-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->