# <a name="add-attachment"></a><span data-ttu-id="1e8ac-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="1e8ac-101">Add attachment</span></span>

<span data-ttu-id="1e8ac-102">С помощью этого API можно создать экземпляр Attachment.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-102">Use this API to create a new Attachment.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e8ac-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e8ac-103">Permissions</span></span>
<span data-ttu-id="1e8ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e8ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e8ac-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e8ac-106">Permission type</span></span>      | <span data-ttu-id="1e8ac-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e8ac-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1e8ac-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e8ac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1e8ac-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e8ac-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="1e8ac-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e8ac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e8ac-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e8ac-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="1e8ac-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e8ac-112">Application</span></span> | <span data-ttu-id="1e8ac-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e8ac-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1e8ac-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e8ac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="1e8ac-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e8ac-115">Request headers</span></span>
| <span data-ttu-id="1e8ac-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1e8ac-116">Name</span></span>       | <span data-ttu-id="1e8ac-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1e8ac-117">Type</span></span> | <span data-ttu-id="1e8ac-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1e8ac-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e8ac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e8ac-119">Authorization</span></span>  | <span data-ttu-id="1e8ac-120">string</span><span class="sxs-lookup"><span data-stu-id="1e8ac-120">string</span></span>  | <span data-ttu-id="1e8ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e8ac-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e8ac-123">Content-Type</span></span> | <span data-ttu-id="1e8ac-124">string</span><span class="sxs-lookup"><span data-stu-id="1e8ac-124">string</span></span>  | <span data-ttu-id="1e8ac-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e8ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e8ac-127">Request body</span></span>
<span data-ttu-id="1e8ac-128">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-128">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1e8ac-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e8ac-129">Response</span></span>

<span data-ttu-id="1e8ac-130">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-130">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="1e8ac-131">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="1e8ac-131">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="1e8ac-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e8ac-132">Request</span></span>
<span data-ttu-id="1e8ac-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="1e8ac-134">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1e8ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e8ac-135">Response</span></span>
<span data-ttu-id="1e8ac-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="1e8ac-139">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="1e8ac-139">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="1e8ac-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e8ac-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="1e8ac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e8ac-141">Response</span></span>
<span data-ttu-id="1e8ac-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1e8ac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
