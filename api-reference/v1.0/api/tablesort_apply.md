# <a name="tablesort-apply"></a><span data-ttu-id="81166-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="81166-101">TableSort: apply</span></span>

<span data-ttu-id="81166-102">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="81166-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="81166-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81166-103">Permissions</span></span>
<span data-ttu-id="81166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81166-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81166-106">Permission type</span></span>      | <span data-ttu-id="81166-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81166-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81166-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81166-108">Delegated (work or school account)</span></span> | <span data-ttu-id="81166-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81166-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81166-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81166-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81166-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81166-111">Not supported.</span></span>    |
|<span data-ttu-id="81166-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81166-112">Application</span></span> | <span data-ttu-id="81166-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81166-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81166-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81166-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="81166-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81166-115">Request headers</span></span>
| <span data-ttu-id="81166-116">Имя</span><span class="sxs-lookup"><span data-stu-id="81166-116">Name</span></span>       | <span data-ttu-id="81166-117">Описание</span><span class="sxs-lookup"><span data-stu-id="81166-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81166-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81166-118">Authorization</span></span>  | <span data-ttu-id="81166-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81166-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81166-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81166-121">Request body</span></span>
<span data-ttu-id="81166-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="81166-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81166-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="81166-123">Parameter</span></span>    | <span data-ttu-id="81166-124">Тип</span><span class="sxs-lookup"><span data-stu-id="81166-124">Type</span></span>   |<span data-ttu-id="81166-125">Описание</span><span class="sxs-lookup"><span data-stu-id="81166-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81166-126">fields</span><span class="sxs-lookup"><span data-stu-id="81166-126">fields</span></span>|<span data-ttu-id="81166-127">SortField</span><span class="sxs-lookup"><span data-stu-id="81166-127">SortField</span></span>|<span data-ttu-id="81166-128">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="81166-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="81166-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="81166-129">matchCase</span></span>|<span data-ttu-id="81166-130">boolean</span><span class="sxs-lookup"><span data-stu-id="81166-130">boolean</span></span>|<span data-ttu-id="81166-p103">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="81166-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="81166-133">method</span><span class="sxs-lookup"><span data-stu-id="81166-133">method</span></span>|<span data-ttu-id="81166-134">string</span><span class="sxs-lookup"><span data-stu-id="81166-134">string</span></span>|<span data-ttu-id="81166-p104">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="81166-p104">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="81166-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="81166-138">Response</span></span>

<span data-ttu-id="81166-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="81166-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81166-141">Пример</span><span class="sxs-lookup"><span data-stu-id="81166-141">Example</span></span>
<span data-ttu-id="81166-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="81166-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81166-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="81166-143">Request</span></span>
<span data-ttu-id="81166-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81166-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="81166-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="81166-145">Response</span></span>
<span data-ttu-id="81166-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="81166-146">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->