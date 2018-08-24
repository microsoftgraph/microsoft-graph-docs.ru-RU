# <a name="message-copy"></a><span data-ttu-id="7bf9b-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="7bf9b-101">message: copy</span></span>

<span data-ttu-id="7bf9b-102">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf9b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf9b-103">Permissions</span></span>

<span data-ttu-id="7bf9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bf9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7bf9b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf9b-106">Permission type</span></span> | <span data-ttu-id="7bf9b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bf9b-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="7bf9b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bf9b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7bf9b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf9b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7bf9b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bf9b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bf9b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf9b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7bf9b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bf9b-112">Application</span></span> | <span data-ttu-id="7bf9b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf9b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf9b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bf9b-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="7bf9b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bf9b-115">Request headers</span></span>

| <span data-ttu-id="7bf9b-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bf9b-116">Header</span></span> | <span data-ttu-id="7bf9b-117">Значение</span><span class="sxs-lookup"><span data-stu-id="7bf9b-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="7bf9b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bf9b-118">Authorization</span></span> | <span data-ttu-id="7bf9b-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-119"></span></span> <span data-ttu-id="7bf9b-120">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-120">Required.</span></span> |
| <span data-ttu-id="7bf9b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bf9b-121">Content-Type</span></span> | <span data-ttu-id="7bf9b-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-122"></span></span> <span data-ttu-id="7bf9b-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bf9b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bf9b-124">Request body</span></span>

<span data-ttu-id="7bf9b-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7bf9b-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="7bf9b-126">Parameter</span></span> | <span data-ttu-id="7bf9b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7bf9b-127">Type</span></span> | <span data-ttu-id="7bf9b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7bf9b-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="7bf9b-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="7bf9b-129">destinationId</span></span>|<span data-ttu-id="7bf9b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="7bf9b-130">String</span></span>|<span data-ttu-id="7bf9b-131">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="7bf9b-132">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7bf9b-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7bf9b-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bf9b-133">Response</span></span>

<span data-ttu-id="7bf9b-134">При успешном выполнении этот метод возвращает код отклика `201 Created` и ресурс [сообщения](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-134">If successful, this method returns a `201 Created` response code and a [sharedDriveItem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf9b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7bf9b-135">Example</span></span>

<span data-ttu-id="7bf9b-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7bf9b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bf9b-137">Request</span></span>
<span data-ttu-id="7bf9b-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="7bf9b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bf9b-139">Response</span></span>

<span data-ttu-id="7bf9b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-140">Here is an example of the response.</span></span>

> <span data-ttu-id="7bf9b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bf9b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
