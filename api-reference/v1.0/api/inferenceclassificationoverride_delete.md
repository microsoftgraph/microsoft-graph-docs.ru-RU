# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="013b8-101">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="013b8-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="013b8-102">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="013b8-102">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="013b8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="013b8-103">Permissions</span></span>
<span data-ttu-id="013b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="013b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="013b8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="013b8-106">Permission type</span></span>      | <span data-ttu-id="013b8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="013b8-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="013b8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="013b8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="013b8-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="013b8-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="013b8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="013b8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="013b8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="013b8-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="013b8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="013b8-112">Application</span></span> | <span data-ttu-id="013b8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="013b8-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="013b8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="013b8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="013b8-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="013b8-115">Request headers</span></span>
| <span data-ttu-id="013b8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="013b8-116">Name</span></span>       | <span data-ttu-id="013b8-117">Тип</span><span class="sxs-lookup"><span data-stu-id="013b8-117">Type</span></span> | <span data-ttu-id="013b8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="013b8-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="013b8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="013b8-119">Authorization</span></span>  | <span data-ttu-id="013b8-120">string</span><span class="sxs-lookup"><span data-stu-id="013b8-120">string</span></span>  | <span data-ttu-id="013b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="013b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="013b8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="013b8-123">Request body</span></span>
<span data-ttu-id="013b8-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="013b8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="013b8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="013b8-125">Response</span></span>

<span data-ttu-id="013b8-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="013b8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013b8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="013b8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="013b8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="013b8-129">Request</span></span>
<span data-ttu-id="013b8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="013b8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="013b8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="013b8-131">Response</span></span>
<span data-ttu-id="013b8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="013b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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