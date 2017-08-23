# <a name="section-copytosectiongroup"></a><span data-ttu-id="f41cd-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f41cd-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="f41cd-102">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="f41cd-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="f41cd-103">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="f41cd-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="f41cd-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f41cd-104">Permissions</span></span>
<span data-ttu-id="f41cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f41cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f41cd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f41cd-107">Permission type</span></span>      | <span data-ttu-id="f41cd-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f41cd-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f41cd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f41cd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f41cd-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41cd-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f41cd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f41cd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f41cd-112">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f41cd-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f41cd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f41cd-113">Application</span></span> | <span data-ttu-id="f41cd-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41cd-114">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f41cd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f41cd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="f41cd-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f41cd-116">Request headers</span></span>
| <span data-ttu-id="f41cd-117">Имя</span><span class="sxs-lookup"><span data-stu-id="f41cd-117">Name</span></span>       | <span data-ttu-id="f41cd-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f41cd-118">Type</span></span> | <span data-ttu-id="f41cd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f41cd-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f41cd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41cd-120">Authorization</span></span>  | <span data-ttu-id="f41cd-121">string</span><span class="sxs-lookup"><span data-stu-id="f41cd-121">string</span></span>  | <span data-ttu-id="f41cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f41cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f41cd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f41cd-124">Content-Type</span></span> | <span data-ttu-id="f41cd-125">строка</span><span class="sxs-lookup"><span data-stu-id="f41cd-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f41cd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f41cd-126">Request body</span></span>
<span data-ttu-id="f41cd-127">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="f41cd-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="f41cd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="f41cd-128">Parameter</span></span>    | <span data-ttu-id="f41cd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f41cd-129">Type</span></span>   |<span data-ttu-id="f41cd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f41cd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f41cd-131">groupId</span><span class="sxs-lookup"><span data-stu-id="f41cd-131">groupId</span></span>|<span data-ttu-id="f41cd-132">String</span><span class="sxs-lookup"><span data-stu-id="f41cd-132">String</span></span>|<span data-ttu-id="f41cd-p103">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="f41cd-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="f41cd-135">id</span><span class="sxs-lookup"><span data-stu-id="f41cd-135">id</span></span>|<span data-ttu-id="f41cd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f41cd-136">String</span></span>|<span data-ttu-id="f41cd-p104">Обязательный. Идентификатор целевой группы разделов.</span><span class="sxs-lookup"><span data-stu-id="f41cd-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="f41cd-139">renameAs</span><span class="sxs-lookup"><span data-stu-id="f41cd-139">renameAs</span></span>|<span data-ttu-id="f41cd-140">String</span><span class="sxs-lookup"><span data-stu-id="f41cd-140">String</span></span>|<span data-ttu-id="f41cd-p105">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="f41cd-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="f41cd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41cd-143">Response</span></span>

<span data-ttu-id="f41cd-p106">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="f41cd-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="f41cd-146">Пример</span><span class="sxs-lookup"><span data-stu-id="f41cd-146">Example</span></span>
<span data-ttu-id="f41cd-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f41cd-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f41cd-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f41cd-148">Request</span></span>
<span data-ttu-id="f41cd-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f41cd-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="f41cd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41cd-150">Response</span></span>
<span data-ttu-id="f41cd-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f41cd-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->