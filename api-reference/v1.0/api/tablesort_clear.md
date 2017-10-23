# <a name="tablesort-clear"></a><span data-ttu-id="c44e5-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="c44e5-101">TableSort: clear</span></span>

<span data-ttu-id="c44e5-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="c44e5-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="c44e5-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c44e5-104">Permissions</span></span>
<span data-ttu-id="c44e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c44e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c44e5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c44e5-107">Permission type</span></span>      | <span data-ttu-id="c44e5-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c44e5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c44e5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c44e5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c44e5-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c44e5-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c44e5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c44e5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c44e5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c44e5-112">Not supported.</span></span>    |
|<span data-ttu-id="c44e5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c44e5-113">Application</span></span> | <span data-ttu-id="c44e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c44e5-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c44e5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c44e5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="c44e5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c44e5-116">Request headers</span></span>
| <span data-ttu-id="c44e5-117">Имя</span><span class="sxs-lookup"><span data-stu-id="c44e5-117">Name</span></span>       | <span data-ttu-id="c44e5-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c44e5-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c44e5-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c44e5-119">Authorization</span></span>  | <span data-ttu-id="c44e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c44e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c44e5-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c44e5-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c44e5-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="c44e5-123">Response</span></span>

<span data-ttu-id="c44e5-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c44e5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c44e5-126">Пример</span><span class="sxs-lookup"><span data-stu-id="c44e5-126">Example</span></span>
<span data-ttu-id="c44e5-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c44e5-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c44e5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c44e5-128">Request</span></span>
<span data-ttu-id="c44e5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c44e5-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="c44e5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c44e5-130">Response</span></span>
<span data-ttu-id="c44e5-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c44e5-131">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->