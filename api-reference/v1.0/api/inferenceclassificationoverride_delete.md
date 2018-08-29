# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="5db3f-101">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="5db3f-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="5db3f-102">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="5db3f-102">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="5db3f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5db3f-103">Permissions</span></span>
<span data-ttu-id="5db3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5db3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5db3f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db3f-106">Permission type</span></span>      | <span data-ttu-id="5db3f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db3f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5db3f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db3f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5db3f-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5db3f-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5db3f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db3f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5db3f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5db3f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5db3f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5db3f-112">Application</span></span> | <span data-ttu-id="5db3f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5db3f-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5db3f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db3f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5db3f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5db3f-115">Request headers</span></span>
| <span data-ttu-id="5db3f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="5db3f-116">Name</span></span>       | <span data-ttu-id="5db3f-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5db3f-117">Type</span></span> | <span data-ttu-id="5db3f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5db3f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5db3f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5db3f-119">Authorization</span></span>  | <span data-ttu-id="5db3f-120">строка</span><span class="sxs-lookup"><span data-stu-id="5db3f-120">string</span></span>  | <span data-ttu-id="5db3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5db3f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5db3f-123">Request body</span></span>
<span data-ttu-id="5db3f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5db3f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5db3f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db3f-125">Response</span></span>

<span data-ttu-id="5db3f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5db3f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db3f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5db3f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5db3f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db3f-129">Request</span></span>
<span data-ttu-id="5db3f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db3f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="5db3f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5db3f-131">Response</span></span>
<span data-ttu-id="5db3f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5db3f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->