# <a name="worksheetprotection-protect"></a><span data-ttu-id="f9454-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="f9454-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="f9454-p101">Защита листа. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="f9454-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9454-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9454-104">Permissions</span></span>
<span data-ttu-id="f9454-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9454-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9454-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9454-107">Permission type</span></span>      | <span data-ttu-id="f9454-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9454-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9454-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9454-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f9454-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9454-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9454-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9454-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9454-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9454-112">Not supported.</span></span>    |
|<span data-ttu-id="f9454-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9454-113">Application</span></span> | <span data-ttu-id="f9454-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9454-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9454-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9454-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="f9454-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9454-116">Request headers</span></span>
| <span data-ttu-id="f9454-117">Имя</span><span class="sxs-lookup"><span data-stu-id="f9454-117">Name</span></span>       | <span data-ttu-id="f9454-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f9454-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9454-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9454-119">Authorization</span></span>  | <span data-ttu-id="f9454-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9454-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9454-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9454-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9454-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f9454-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9454-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9454-125">Request body</span></span>
<span data-ttu-id="f9454-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f9454-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9454-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="f9454-127">Parameter</span></span>    | <span data-ttu-id="f9454-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f9454-128">Type</span></span>   |<span data-ttu-id="f9454-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f9454-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9454-130">options</span><span class="sxs-lookup"><span data-stu-id="f9454-130">options</span></span>|<span data-ttu-id="f9454-131">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="f9454-131">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="f9454-p105">Необязательные параметры защиты листа.</span><span class="sxs-lookup"><span data-stu-id="f9454-p105">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="f9454-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9454-134">Response</span></span>

<span data-ttu-id="f9454-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f9454-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9454-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f9454-137">Example</span></span>
<span data-ttu-id="f9454-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f9454-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9454-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9454-139">Request</span></span>
<span data-ttu-id="f9454-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9454-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="f9454-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9454-141">Response</span></span>
<span data-ttu-id="f9454-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9454-142">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
