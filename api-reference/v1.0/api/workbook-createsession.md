---
title: 'книга: createSession'
description: Создание нового сеанса книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f931313e09068892ebbe167ecb85d5577a148f92
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575058"
---
# <a name="workbook-createsession"></a><span data-ttu-id="c153b-103">книга: createSession</span><span class="sxs-lookup"><span data-stu-id="c153b-103">workbook: createSession</span></span>

<span data-ttu-id="c153b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c153b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c153b-105">Создание нового сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="c153b-105">Create a new workbook session.</span></span> 

<span data-ttu-id="c153b-106">Интерфейсы API Excel можно вызвать в одном из двух режимов.</span><span class="sxs-lookup"><span data-stu-id="c153b-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="c153b-p101">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="c153b-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="c153b-p102">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="c153b-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="c153b-113">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="c153b-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="c153b-p103">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="c153b-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

<span data-ttu-id="c153b-117">В некоторых случаях для создания нового сеанса требуется определенное время.</span><span class="sxs-lookup"><span data-stu-id="c153b-117">In some cases, creating a new session requires an indeterminate time to complete.</span></span> <span data-ttu-id="c153b-118">Microsoft Graph также предоставляет длительный шаблон операций.</span><span class="sxs-lookup"><span data-stu-id="c153b-118">Microsoft Graph also provides a long running operations pattern.</span></span> <span data-ttu-id="c153b-119">Этот шаблон позволяет оповещеть об обновлениях состояния создания, не дожидаясь завершения создания.</span><span class="sxs-lookup"><span data-stu-id="c153b-119">This pattern provides a way to poll for creation status updates, without waiting for the creation to complete.</span></span> <span data-ttu-id="c153b-120">Ниже следующую меру:</span><span class="sxs-lookup"><span data-stu-id="c153b-120">The following are the steps:</span></span>

1. <span data-ttu-id="c153b-121">В `Prefer: respond-async` запрос добавляется загон, чтобы указать, что это долгосрочная операция.</span><span class="sxs-lookup"><span data-stu-id="c153b-121">A `Prefer: respond-async` header is added to the request to indicate that it is a long-running operation.</span></span>
2. <span data-ttu-id="c153b-122">Ответ возвращает `Location` заглавную, чтобы указать URL-адрес для опроса состояния операции создания.</span><span class="sxs-lookup"><span data-stu-id="c153b-122">The response returns a `Location` header to specify the URL for polling the creation operation status.</span></span> <span data-ttu-id="c153b-123">Вы можете получить состояние операции, доступ к указанному URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="c153b-123">You can get the operation status by accessing the specified URL.</span></span> <span data-ttu-id="c153b-124">Состояние будет одним из следующих: `notStarted` , , , или `running` `succeeded` `failed` .</span><span class="sxs-lookup"><span data-stu-id="c153b-124">The status will be one of the following: `notStarted`, `running`, `succeeded`, or `failed`.</span></span>
3. <span data-ttu-id="c153b-125">После завершения операции можно снова запросить состояние, и ответ будет либо показываться, либо `succeeded` `failed` .</span><span class="sxs-lookup"><span data-stu-id="c153b-125">After the operation completes, you can request the status again and the response will show either `succeeded` or `failed`.</span></span>

## <a name="error-handling"></a><span data-ttu-id="c153b-126">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="c153b-126">Error handling</span></span>

<span data-ttu-id="c153b-127">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="c153b-127">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="c153b-128">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="c153b-128">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c153b-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c153b-129">Permissions</span></span>
<span data-ttu-id="c153b-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c153b-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c153b-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c153b-132">Permission type</span></span>      | <span data-ttu-id="c153b-133">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c153b-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c153b-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c153b-134">Delegated (work or school account)</span></span> | <span data-ttu-id="c153b-135">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c153b-135">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c153b-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c153b-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c153b-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c153b-137">Not supported.</span></span>    |
|<span data-ttu-id="c153b-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c153b-138">Application</span></span> | <span data-ttu-id="c153b-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c153b-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c153b-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c153b-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/createSession
POST /me/drive/root:/{item-path}:/workbook/createSession
```
## <a name="request-headers"></a><span data-ttu-id="c153b-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c153b-141">Request headers</span></span>
| <span data-ttu-id="c153b-142">Имя</span><span class="sxs-lookup"><span data-stu-id="c153b-142">Name</span></span>       | <span data-ttu-id="c153b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="c153b-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c153b-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c153b-144">Authorization</span></span>  | <span data-ttu-id="c153b-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c153b-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c153b-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c153b-147">Request body</span></span>
<span data-ttu-id="c153b-148">В теле запроса поставляем представление JSON объекта [workbookSessionInfo.](../resources/workbooksessioninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c153b-148">In the request body, supply a JSON representation of [workbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c153b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c153b-149">Response</span></span>

<span data-ttu-id="c153b-150">В случае успеха этот метод возвращает код ответа и объект `201 Created` [workbookSessionInfo](../resources/workbooksessioninfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c153b-150">If successful, this method returns a `201 Created` response code and a [workbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span> <span data-ttu-id="c153b-151">Для длительной операции возвращается код ответа и заголовка с `202 Accepted ` `Location` пустым телом в ответе.</span><span class="sxs-lookup"><span data-stu-id="c153b-151">For a long-running operation, it returns a `202 Accepted ` response code and a `Location` header with an empty body in the response.</span></span>

## <a name="examples"></a><span data-ttu-id="c153b-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="c153b-152">Examples</span></span>

### <a name="example-1-basic-session-creation"></a><span data-ttu-id="c153b-153">Пример 1. Создание базового сеанса</span><span class="sxs-lookup"><span data-stu-id="c153b-153">Example 1: Basic session creation</span></span>
#### <a name="request"></a><span data-ttu-id="c153b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c153b-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c153b-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="c153b-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[<span data-ttu-id="c153b-156">C#</span><span class="sxs-lookup"><span data-stu-id="c153b-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c153b-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c153b-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c153b-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c153b-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c153b-159">Java</span><span class="sxs-lookup"><span data-stu-id="c153b-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c153b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c153b-160">Response</span></span>
><span data-ttu-id="c153b-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c153b-161">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "persistChanges": true
}
```

### <a name="example-2-session-creation-with-long-running-operation-pattern"></a><span data-ttu-id="c153b-162">Пример 2. Создание сеанса с длительным шаблоном работы</span><span class="sxs-lookup"><span data-stu-id="c153b-162">Example 2: Session creation with long-running operation pattern</span></span>

#### <a name="request"></a><span data-ttu-id="c153b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c153b-163">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a><span data-ttu-id="c153b-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c153b-164">Response</span></span>
><span data-ttu-id="c153b-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c153b-165">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

