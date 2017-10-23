# <a name="create-session"></a><span data-ttu-id="ab93c-101">Create Session</span><span class="sxs-lookup"><span data-stu-id="ab93c-101">Create Session</span></span>

<span data-ttu-id="ab93c-102">Используйте этот API для создания сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="ab93c-102">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="ab93c-103">API Excel можно вызвать в одном из двух режимов:</span><span class="sxs-lookup"><span data-stu-id="ab93c-103">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="ab93c-p101">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="ab93c-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="ab93c-p102">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="ab93c-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="ab93c-110">Чтобы представить сеанс в API, воспользуйтесь заголовком `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="ab93c-110">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="ab93c-p103">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="ab93c-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="permissions"></a><span data-ttu-id="ab93c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab93c-114">Permissions</span></span>
<span data-ttu-id="ab93c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab93c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab93c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab93c-117">Permission type</span></span>      | <span data-ttu-id="ab93c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab93c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab93c-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab93c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ab93c-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab93c-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab93c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab93c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab93c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab93c-122">Not supported.</span></span>    |
|<span data-ttu-id="ab93c-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab93c-123">Application</span></span> | <span data-ttu-id="ab93c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab93c-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab93c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab93c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="ab93c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab93c-126">Request headers</span></span>
| <span data-ttu-id="ab93c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="ab93c-127">Name</span></span>       | <span data-ttu-id="ab93c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ab93c-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab93c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab93c-129">Authorization</span></span>  | <span data-ttu-id="ab93c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab93c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab93c-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab93c-132">Request body</span></span>
<span data-ttu-id="ab93c-133">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="ab93c-133">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab93c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab93c-134">Response</span></span>

<span data-ttu-id="ab93c-135">При успешном выполнении этот метод возвращает код ответа `201 Created` и объект [WorkbookSessionInfo](../resources/workbooksessioninfo.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab93c-135">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab93c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ab93c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab93c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab93c-137">Request</span></span>
<span data-ttu-id="ab93c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab93c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistSession": true
}
```
<span data-ttu-id="ab93c-139">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="ab93c-139">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ab93c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab93c-140">Response</span></span>
<span data-ttu-id="ab93c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab93c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistSession": true
}
```

