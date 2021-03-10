---
title: Работа с Excel в Microsoft Graph
description: С помощью Microsoft Graph можно разрешать веб-приложениям и мобильным приложениям считывать и изменять книги Excel, хранящиеся в OneDrive для бизнеса, на сайте SharePoint или диске группы.
localization_priority: Priority
author: grangery
ms.prod: excel
doc_type: conceptualPageType
ms.openlocfilehash: 2fe503472021c26c2ec856e1b73cb9f432190891
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576003"
---
# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="7692a-103">Работа с Excel в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7692a-103">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="7692a-p101">Можно использовать Microsoft Graph, чтобы разрешать веб-приложениям и мобильным приложениям считывать и изменять книги Excel, хранящиеся в OneDrive для бизнеса, на сайте SharePoint или диске группы. Ресурс `Workbook` (или файл Excel) содержит все остальные ресурсы Excel благодаря отношениям. Можно получить доступ к книге через интерфейс [API Drive](drive.md), указав расположение файла в URL-адресе. Пример:</span><span class="sxs-lookup"><span data-stu-id="7692a-p101">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive for Business, SharePoint site or Group drive. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="7692a-p102">Можно получить доступ к набору объектов Excel (например, Table, Range или Chart) с помощью стандартных интерфейсов API REST, чтобы выполнять в книге операции создания, чтения, обновления и удаления (CRUD). Например, `GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="7692a-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="7692a-110">возвращает коллекцию объектов листа, включенных в книгу.</span><span class="sxs-lookup"><span data-stu-id="7692a-110">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="7692a-p103">REST API Excel поддерживает только книги в формате Office Open XML. Книги с расширением `.xls` не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="7692a-p103">The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

<span data-ttu-id="7692a-113">**Примечание.** Поддержка книг, хранящихся в обычном OneDrive, по-прежнему недоступна.</span><span class="sxs-lookup"><span data-stu-id="7692a-113">**Note**: Support for workbooks stored in OneDrive Consumer platform is still not available.</span></span> <span data-ttu-id="7692a-114">В настоящее время REST API Excel поддерживаются только файлы, хранящиеся в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7692a-114">At this time, only the files stored in business platform is supported by Excel REST APIs.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="7692a-115">Авторизация и области</span><span class="sxs-lookup"><span data-stu-id="7692a-115">Authorization and scopes</span></span>

<span data-ttu-id="7692a-116">Для проверки подлинности API Excel вы можете использовать [конечную точку Azure AD версии 2](../index.md).</span><span class="sxs-lookup"><span data-stu-id="7692a-116">You can use the [Azure AD v.2 endpoint](../index.md) to authenticate Excel APIs.</span></span> <span data-ttu-id="7692a-117">Для всех API требуется заголовок HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="7692a-117">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="7692a-118">Чтобы использовать ресурс Excel, требуется одно из следующих [разрешений](/graph/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="7692a-118">One of the following [permission scopes](/graph/permissions-reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="7692a-119">Files.Read (для чтения)</span><span class="sxs-lookup"><span data-stu-id="7692a-119">Files.Read (for read actions)</span></span>
* <span data-ttu-id="7692a-120">Files.ReadWrite (для чтения и записи)</span><span class="sxs-lookup"><span data-stu-id="7692a-120">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="7692a-121">Сеансы и сохраняемость</span><span class="sxs-lookup"><span data-stu-id="7692a-121">Sessions and persistence</span></span>

<span data-ttu-id="7692a-122">API Excel можно вызвать в одном из трех режимов:</span><span class="sxs-lookup"><span data-stu-id="7692a-122">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="7692a-123">Сохраняемый сеанс: все изменения, внесенные в книгу, сохраняются (записываются).</span><span class="sxs-lookup"><span data-stu-id="7692a-123">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="7692a-124">Это наиболее эффективный и производительный режим работы.</span><span class="sxs-lookup"><span data-stu-id="7692a-124">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="7692a-p107">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="7692a-p107">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="7692a-129">Без сеанса: вызов API выполняется без сведений о сеансе.</span><span class="sxs-lookup"><span data-stu-id="7692a-129">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="7692a-130">Чтобы выполнить операцию, серверам Excel каждый раз необходимо находить копию книги на сервере, и, соответственно, это неэффективный способ вызова API Excel.</span><span class="sxs-lookup"><span data-stu-id="7692a-130">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="7692a-131">Он подходит для выполнения одиночных запросов.</span><span class="sxs-lookup"><span data-stu-id="7692a-131">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="7692a-132">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="7692a-132">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="7692a-p109">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="7692a-p109">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="7692a-136">Вызов API для получения сеанса</span><span class="sxs-lookup"><span data-stu-id="7692a-136">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="7692a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-137">Request</span></span> 

<span data-ttu-id="7692a-138">Передайте объект JSON, установив для параметра `persistchanges` значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="7692a-138">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="7692a-139">Если для параметра `persistChanges` установлено значение `false`, возвращается идентификатор непостоянного сеанса.</span><span class="sxs-lookup"><span data-stu-id="7692a-139">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="7692a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-140">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="7692a-141">Применение</span><span class="sxs-lookup"><span data-stu-id="7692a-141">Usage</span></span> 

<span data-ttu-id="7692a-142">Идентификатор сеанса, возвращенный из предыдущего вызова, передается в качестве заголовка при последующих запросах API в</span><span class="sxs-lookup"><span data-stu-id="7692a-142">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="7692a-143">заголовке HTTP `workbook-session-id`.</span><span class="sxs-lookup"><span data-stu-id="7692a-143">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="7692a-144">Примечание. Если срок действия идентификатора сеанса истек, для сеанса будет возвращен код ошибки HTTP `404`.</span><span class="sxs-lookup"><span data-stu-id="7692a-144">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="7692a-145">В таком случае вы можете создать другой сеанс и продолжить работу.</span><span class="sxs-lookup"><span data-stu-id="7692a-145">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="7692a-146">Можно использовать другой подход — периодически обновлять сеанс, чтобы он не был завершен.</span><span class="sxs-lookup"><span data-stu-id="7692a-146">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="7692a-147">Обычно срок действия сохраняемого сеанса истекает через 5 минут бездействия.</span><span class="sxs-lookup"><span data-stu-id="7692a-147">Typically the persistent session expires after about 5 minutes of inactivity.</span></span> <span data-ttu-id="7692a-148">Срок действия несохраняемого сеанса истекает через 7 минут бездействия.</span><span class="sxs-lookup"><span data-stu-id="7692a-148">Non persistent session expires after about 7 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="7692a-149">Стандартные сценарии Excel</span><span class="sxs-lookup"><span data-stu-id="7692a-149">Common Excel scenarios</span></span>

<span data-ttu-id="7692a-150">В этом разделе приводятся примеры использования стандартных операций для объектов Excel.</span><span class="sxs-lookup"><span data-stu-id="7692a-150">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="7692a-151">Операции с листами</span><span class="sxs-lookup"><span data-stu-id="7692a-151">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="7692a-152">Список листов, являющихся частью книги</span><span class="sxs-lookup"><span data-stu-id="7692a-152">List worksheets part of the workbook</span></span> 
<span data-ttu-id="7692a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-153">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-154">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="7692a-155">Добавление листа</span><span class="sxs-lookup"><span data-stu-id="7692a-155">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/root:/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="7692a-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="7692a-156">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="7692a-157">Получение нового листа</span><span class="sxs-lookup"><span data-stu-id="7692a-157">Get a new worksheet</span></span> 

<span data-ttu-id="7692a-158">Получение листа по его имени.</span><span class="sxs-lookup"><span data-stu-id="7692a-158">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7692a-159">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="7692a-p111">\*\* Примечание. Листы также можно получать, используя идентификатор. Однако в настоящее время идентификатор содержит символы `{` и "}", поэтому необходимо использовать кодировку URL, чтобы API работал. Пример. Чтобы получить лист с идентификатором `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, преобразуйте идентификатор в путь URL: `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="7692a-p111">\*\* Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="7692a-163">Удаление листа</span><span class="sxs-lookup"><span data-stu-id="7692a-163">Delete a worksheet</span></span>

<span data-ttu-id="7692a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-164">Request</span></span>
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-165">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="7692a-166">Обновление свойств листа</span><span class="sxs-lookup"><span data-stu-id="7692a-166">Update worksheet properties</span></span>

<span data-ttu-id="7692a-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-167">Request</span></span> 

```
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="7692a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-168">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="7692a-169">Операции с диаграммами</span><span class="sxs-lookup"><span data-stu-id="7692a-169">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="7692a-170">Список диаграмм, являющихся частью листа</span><span class="sxs-lookup"><span data-stu-id="7692a-170">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="7692a-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-171">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="7692a-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-172">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="7692a-p112">\*\* Примечание. Идентификатор диаграмма содержит символы `{` и `}` (пример: `{00000000-0008-0000-0100-000003000000}`), поэтому необходимо использовать кодировку URL, чтобы API работал. Пример. Чтобы получить объект диаграммы, преобразуйте идентификатор в путь URL: `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="7692a-p112">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="7692a-175">Получение изображения диаграммы</span><span class="sxs-lookup"><span data-stu-id="7692a-175">Get chart image</span></span>

<span data-ttu-id="7692a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-176">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="7692a-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-177">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="7692a-178">Добавление диаграммы</span><span class="sxs-lookup"><span data-stu-id="7692a-178">Add a chart</span></span>  

<span data-ttu-id="7692a-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-179">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="7692a-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-180">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chart",
  "@odata.type": "#microsoft.graph.workbookChart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="7692a-181">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="7692a-181">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="7692a-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-182">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="7692a-183">Обновление исходных данных диаграммы</span><span class="sxs-lookup"><span data-stu-id="7692a-183">Update chart source data</span></span> 

<span data-ttu-id="7692a-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-184">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="7692a-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-185">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="7692a-186">Операции с таблицей</span><span class="sxs-lookup"><span data-stu-id="7692a-186">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="7692a-187">Получение списка таблиц</span><span class="sxs-lookup"><span data-stu-id="7692a-187">Get list of tables</span></span> 

<span data-ttu-id="7692a-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-188">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-189">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="7692a-190">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-190">Create table</span></span>

<span data-ttu-id="7692a-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-191">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/{table-id}/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="7692a-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-192">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a><span data-ttu-id="7692a-193">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-193">Update table</span></span>

<span data-ttu-id="7692a-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-194">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="7692a-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-195">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="7692a-196">Получение списка строк таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-196">Get list of table rows</span></span>
<span data-ttu-id="7692a-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-197">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-198">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="7692a-199">Получение списка столбцов таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-199">Get list of table columns</span></span>

<span data-ttu-id="7692a-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-200">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-201">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="7692a-202">Добавление строки таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-202">Add a table row</span></span>

<span data-ttu-id="7692a-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-203">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="7692a-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-204">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="7692a-205">Добавление столбца таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-205">Add a table column</span></span> 

<span data-ttu-id="7692a-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-206">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="7692a-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-207">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="7692a-208">Удаление строки таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-208">Delete table row</span></span>

<span data-ttu-id="7692a-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-209">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http  
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows/$/itemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-210">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="7692a-211">Удаление столбца таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-211">Delete table column</span></span> 
<span data-ttu-id="7692a-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-212">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-213">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="7692a-214">Преобразование таблицы в диапазон</span><span class="sxs-lookup"><span data-stu-id="7692a-214">Convert table to range</span></span> 
<span data-ttu-id="7692a-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-215">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-216">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="7692a-217">Сортировка таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-217">Table sort</span></span>
<span data-ttu-id="7692a-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-218">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="7692a-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-219">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="7692a-220">Фильтрация таблицы</span><span class="sxs-lookup"><span data-stu-id="7692a-220">Table filter</span></span>
<span data-ttu-id="7692a-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-221">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="7692a-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-222">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="7692a-223">Очистка фильтра</span><span class="sxs-lookup"><span data-stu-id="7692a-223">Clear filter</span></span>
<span data-ttu-id="7692a-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-224">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-225">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="7692a-226">Операции с диапазоном</span><span class="sxs-lookup"><span data-stu-id="7692a-226">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="7692a-227">Получение диапазона</span><span class="sxs-lookup"><span data-stu-id="7692a-227">Get Range</span></span> 

<span data-ttu-id="7692a-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-228">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-229">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="7692a-230">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="7692a-230">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="7692a-231">Сортировка диапазона</span><span class="sxs-lookup"><span data-stu-id="7692a-231">Range sort</span></span>
<span data-ttu-id="7692a-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-232">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="7692a-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-233">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="7692a-234">Именованные элементы</span><span class="sxs-lookup"><span data-stu-id="7692a-234">Named items</span></span>
<span data-ttu-id="7692a-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-235">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="7692a-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-236">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="7692a-237">Работа со значениями null</span><span class="sxs-lookup"><span data-stu-id="7692a-237">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="7692a-238">Входное значение null в двумерном массиве</span><span class="sxs-lookup"><span data-stu-id="7692a-238">null input in 2-D array</span></span>

<span data-ttu-id="7692a-p113">Входное значение `null` в двумерном массиве (для значений, числового формата, формулы) игнорируется в ресурсах Range и Table. Предполагаемый целевой объект (ячейка) не будет обновлен, если входное значение `null` отправлено в виде значений, числового формата или сетки значений формулы.</span><span class="sxs-lookup"><span data-stu-id="7692a-p113">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="7692a-241">Например, чтобы обновить только определенные части Range, такие как числовой формат ячейки, и сохранить существующий числовой формат в других частях Range, установите числовой формат там, где это необходимо, и отправьте `null` для других ячеек.</span><span class="sxs-lookup"><span data-stu-id="7692a-241">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="7692a-242">В приведенном ниже запросе задаются только некоторые значения числового формата Range, в то время как в остальных случаях сохраняется имеющийся числовой формат (передаются значения null).</span><span class="sxs-lookup"><span data-stu-id="7692a-242">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="7692a-243">Входное значение null для свойства</span><span class="sxs-lookup"><span data-stu-id="7692a-243">null input for a property</span></span>

<span data-ttu-id="7692a-p114">`null` не является допустимым входным значением для всего свойства. Например, следующий пример недопустим, так как целые значения нельзя устанавливать на null или игнорировать.</span><span class="sxs-lookup"><span data-stu-id="7692a-p114">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="7692a-246">Следующий пример также недопустим, потому что значение null недопустимо для цвета.</span><span class="sxs-lookup"><span data-stu-id="7692a-246">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="7692a-247">Отклик — null</span><span class="sxs-lookup"><span data-stu-id="7692a-247">Null-Response</span></span>

<span data-ttu-id="7692a-248">Представление свойств форматирования, состоящее из неоднородных значений, приведет к возврату значения null в отклике.</span><span class="sxs-lookup"><span data-stu-id="7692a-248">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="7692a-p115">Например, Range может состоять из одной или нескольких ячеек. Если отдельные ячейки в указанном объекте Range не содержат единообразных значений форматирования, представление уровня диапазона будет неопределенным.</span><span class="sxs-lookup"><span data-stu-id="7692a-p115">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```

<span data-ttu-id="7692a-251">Значение null также возвращается в отклике в указанных ниже случаях.</span><span class="sxs-lookup"><span data-stu-id="7692a-251">A null value is also returned in the response in the following cases:</span></span>
- <span data-ttu-id="7692a-252">Если при попытке получить определенное свойство объекта возникает ошибка, и для такого свойства можно задать значение null, свойство может возвращать в отклике значение null.</span><span class="sxs-lookup"><span data-stu-id="7692a-252">If an error occurs when trying to get a certain property of an object and this property can be set as a null, the property might return a null value in the response.</span></span>
- <span data-ttu-id="7692a-253">Для объекта Range при получении диапазона для целой строки или целого столбца некоторые свойства могут возвращать значение null в качестве отклика.</span><span class="sxs-lookup"><span data-stu-id="7692a-253">For a range object, when getting a range for entire row or entire column, some properties might return null as the response.</span></span> <span data-ttu-id="7692a-254">Если размер диапазона превышает верхнее ограничение (5 млн ячеек), некоторые свойства возвращают null в качестве значения.</span><span class="sxs-lookup"><span data-stu-id="7692a-254">If the range size exceeds the upper limitation (5M cells), some properties will return null as the value.</span></span>

### <a name="blank-input-and-output"></a><span data-ttu-id="7692a-255">Пустые входные и выходные данные</span><span class="sxs-lookup"><span data-stu-id="7692a-255">Blank input and output</span></span>

<span data-ttu-id="7692a-p117">Пустые значения в запросах на обновление считаются указанием на очистку или сброс соответствующего свойства. Пустое значение представляется двумя двойными кавычками, не разделенными пробелом: `""`</span><span class="sxs-lookup"><span data-stu-id="7692a-p117">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="7692a-258">Примеры:</span><span class="sxs-lookup"><span data-stu-id="7692a-258">Examples:</span></span>

* <span data-ttu-id="7692a-259">Для `values` значение диапазона очищено. Это аналогично очистке содержимого в приложении.</span><span class="sxs-lookup"><span data-stu-id="7692a-259">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="7692a-260">Для `numberFormat` числовому формату присвоено значение `General`.</span><span class="sxs-lookup"><span data-stu-id="7692a-260">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="7692a-261">Для `formula` и `formulaLocale` значения формулы очищены.</span><span class="sxs-lookup"><span data-stu-id="7692a-261">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="7692a-p118">При операциях чтения будьте готовы получать пустые значения, если в ячейках нет содержимого. Если ячейка не содержит данных или значений, API возвращает пустое значение. Пустое значение представляется двумя двойными кавычками, не разделенными пробелом: `""`</span><span class="sxs-lookup"><span data-stu-id="7692a-p118">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="7692a-265">Range без ограничений</span><span class="sxs-lookup"><span data-stu-id="7692a-265">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="7692a-266">Чтение</span><span class="sxs-lookup"><span data-stu-id="7692a-266">Read</span></span>

<span data-ttu-id="7692a-267">Адрес Range без ограничений содержит только идентификаторы столбцов и строк, а также идентификаторы неопределенных строк и столбцов (соответственно). Пример:</span><span class="sxs-lookup"><span data-stu-id="7692a-267">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="7692a-268">`C:C`, `A:F`, `A:XFD` (содержит неопределенные строки).</span><span class="sxs-lookup"><span data-stu-id="7692a-268">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="7692a-269">`2:2`, `1:4`, `1:1048546` (содержит неопределенные столбцы).</span><span class="sxs-lookup"><span data-stu-id="7692a-269">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="7692a-p119">Когда API запрашивает Range без ограничений (`getRange('C:C')`), отклик содержит значение `null` для свойств на уровне ячеек, например `values`, `text`, `numberFormat` или `formula`. Другие свойства Range, например `address` или `cellCount`, отражают неограниченный диапазон.</span><span class="sxs-lookup"><span data-stu-id="7692a-p119">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="7692a-272">Запись</span><span class="sxs-lookup"><span data-stu-id="7692a-272">Write</span></span>

<span data-ttu-id="7692a-273">Задание свойств уровня ячеек (например, значений, numberFormat и т. д.) для Range без ограничений **не допускается**, так как запрос на ввод может оказаться слишком большим для обработки.</span><span class="sxs-lookup"><span data-stu-id="7692a-273">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="7692a-274">Например, приведенный ниже запрос на обновление значений недопустим, так как запрашиваемый диапазон не ограничен.</span><span class="sxs-lookup"><span data-stu-id="7692a-274">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="7692a-275">Когда для такого объекта Range предпринимается попытка выполнить операцию обновления, API возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="7692a-275">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="7692a-276">Большой диапазон</span><span class="sxs-lookup"><span data-stu-id="7692a-276">Large Range</span></span>

<span data-ttu-id="7692a-p120">Большой диапазон — это объект Range, размер которого слишком велик для одного вызова API. Множество факторов, например количество ячеек, значений, объектов numberFormat и формул, могут сделать запрос настолько большим, что он станет неподходящим для взаимодействия с API. Интерфейс API делает все возможное для возврата запрашиваемых данных или записи в них. Но обработка крупного запроса может привести к ошибке API из-за чрезмерного использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7692a-p120">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="7692a-281">Чтобы избежать этого, рекомендуем выполнять операции чтения и записи для нескольких объектов Range меньшего размера.</span><span class="sxs-lookup"><span data-stu-id="7692a-281">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="7692a-282">Копирование одного входного значения</span><span class="sxs-lookup"><span data-stu-id="7692a-282">Single input copy</span></span>

<span data-ttu-id="7692a-p121">Для поддержки обновления диапазона с использованием одинаковых значений или числового формата либо для применения одной и той же формулы ко всему диапазону в установленном интерфейсе API используется следующее соглашение. В Excel этот принцип аналогичен вводу значений или формул в диапазон в режиме CTRL+ВВОД.</span><span class="sxs-lookup"><span data-stu-id="7692a-p121">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="7692a-285">API ищет *значение одной ячейки* и, если размер целевого диапазона не соответствует размеру входного диапазона, обновление применяется ко всему диапазону в режиме CTRL+ВВОД с использованием значения или формулы в запросе.</span><span class="sxs-lookup"><span data-stu-id="7692a-285">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="7692a-286">Примеры</span><span class="sxs-lookup"><span data-stu-id="7692a-286">Examples</span></span>

<span data-ttu-id="7692a-p122">Следующий запрос добавляет в выбранный диапазон текст "Sample text". Обратите внимание, что Range содержит 200 ячеек, в то время как входные данные — значение лишь для одной ячейки.</span><span class="sxs-lookup"><span data-stu-id="7692a-p122">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="7692a-289">Функции книги</span><span class="sxs-lookup"><span data-stu-id="7692a-289">Workbook functions</span></span> 
<span data-ttu-id="7692a-290">Можно получить доступ к функциям книги через коллекцию функций, включенных в ресурс /Functions.</span><span class="sxs-lookup"><span data-stu-id="7692a-290">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="7692a-291">Запрос</span><span class="sxs-lookup"><span data-stu-id="7692a-291">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="7692a-292">Отклик</span><span class="sxs-lookup"><span data-stu-id="7692a-292">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="7692a-293">Сведения об ошибках</span><span class="sxs-lookup"><span data-stu-id="7692a-293">Error information</span></span> 

<span data-ttu-id="7692a-p123">Ошибки возвращаются с HTTP-кодом и объектом ошибки. Ошибки `code` и `message` объясняют причины возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="7692a-p123">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="7692a-296">Ниже приведен пример.</span><span class="sxs-lookup"><span data-stu-id="7692a-296">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

## <a name="whats-new"></a><span data-ttu-id="7692a-297">Что нового</span><span class="sxs-lookup"><span data-stu-id="7692a-297">What's new</span></span>
<span data-ttu-id="7692a-298">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="7692a-298">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
