# <a name="filter-apply"></a><span data-ttu-id="16cfe-101">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="16cfe-101">Filter: apply</span></span>

<span data-ttu-id="16cfe-102">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="16cfe-102">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="16cfe-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16cfe-103">Permissions</span></span>
<span data-ttu-id="16cfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16cfe-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16cfe-106">Permission type</span></span>      | <span data-ttu-id="16cfe-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16cfe-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16cfe-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16cfe-108">Delegated (work or school account)</span></span> | <span data-ttu-id="16cfe-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16cfe-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16cfe-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16cfe-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16cfe-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cfe-111">Not supported.</span></span>    |
|<span data-ttu-id="16cfe-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16cfe-112">Application</span></span> | <span data-ttu-id="16cfe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cfe-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16cfe-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16cfe-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="16cfe-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16cfe-115">Request headers</span></span>
| <span data-ttu-id="16cfe-116">Имя</span><span class="sxs-lookup"><span data-stu-id="16cfe-116">Name</span></span>       | <span data-ttu-id="16cfe-117">Описание</span><span class="sxs-lookup"><span data-stu-id="16cfe-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16cfe-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16cfe-118">Authorization</span></span>  | <span data-ttu-id="16cfe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16cfe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16cfe-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16cfe-121">Request body</span></span>
<span data-ttu-id="16cfe-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16cfe-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16cfe-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="16cfe-123">Parameter</span></span>    | <span data-ttu-id="16cfe-124">Тип</span><span class="sxs-lookup"><span data-stu-id="16cfe-124">Type</span></span>   |<span data-ttu-id="16cfe-125">Описание</span><span class="sxs-lookup"><span data-stu-id="16cfe-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16cfe-126">criteria</span><span class="sxs-lookup"><span data-stu-id="16cfe-126">criteria</span></span>|<span data-ttu-id="16cfe-127">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="16cfe-127">FilterCriteria</span></span>|<span data-ttu-id="16cfe-128">Применяемые условия.</span><span class="sxs-lookup"><span data-stu-id="16cfe-128">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="16cfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cfe-129">Response</span></span>

<span data-ttu-id="16cfe-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="16cfe-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cfe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="16cfe-132">Example</span></span>
<span data-ttu-id="16cfe-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16cfe-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16cfe-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="16cfe-134">Request</span></span>
<span data-ttu-id="16cfe-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16cfe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="16cfe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cfe-136">Response</span></span>
<span data-ttu-id="16cfe-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16cfe-137">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->