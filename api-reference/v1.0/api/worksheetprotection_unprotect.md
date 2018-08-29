# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="252f4-101">WorksheetProtection: снять защиту</span><span class="sxs-lookup"><span data-stu-id="252f4-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="252f4-102">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="252f4-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="252f4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="252f4-103">Permissions</span></span>
<span data-ttu-id="252f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="252f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="252f4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="252f4-106">Permission type</span></span>      | <span data-ttu-id="252f4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="252f4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="252f4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="252f4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="252f4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="252f4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="252f4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="252f4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="252f4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252f4-111">Not supported.</span></span>    |
|<span data-ttu-id="252f4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="252f4-112">Application</span></span> | <span data-ttu-id="252f4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252f4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="252f4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="252f4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="252f4-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="252f4-115">Request headers</span></span>
| <span data-ttu-id="252f4-116">Имя</span><span class="sxs-lookup"><span data-stu-id="252f4-116">Name</span></span>       | <span data-ttu-id="252f4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="252f4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="252f4-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="252f4-118">Authorization</span></span>  | <span data-ttu-id="252f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="252f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="252f4-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="252f4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="252f4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="252f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="252f4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="252f4-124">Request body</span></span>
<span data-ttu-id="252f4-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="252f4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="252f4-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="252f4-126">Parameter</span></span>    | <span data-ttu-id="252f4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="252f4-127">Type</span></span>   |<span data-ttu-id="252f4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="252f4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="252f4-129">password</span><span class="sxs-lookup"><span data-stu-id="252f4-129">password</span></span>|<span data-ttu-id="252f4-130">строка</span><span class="sxs-lookup"><span data-stu-id="252f4-130">string</span></span>|<span data-ttu-id="252f4-p104">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="252f4-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="252f4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="252f4-133">Response</span></span>

<span data-ttu-id="252f4-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="252f4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="252f4-136">Пример</span><span class="sxs-lookup"><span data-stu-id="252f4-136">Example</span></span>
<span data-ttu-id="252f4-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="252f4-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="252f4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="252f4-138">Request</span></span>
<span data-ttu-id="252f4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="252f4-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="252f4-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="252f4-140">Response</span></span>
<span data-ttu-id="252f4-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="252f4-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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