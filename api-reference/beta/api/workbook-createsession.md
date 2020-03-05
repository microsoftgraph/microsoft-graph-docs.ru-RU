---
title: Create Session
description: 'Используйте этот API для создания сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 27705a8e875b9c78fd5437d4f4704f778d165f00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451518"
---
# <a name="create-session"></a><span data-ttu-id="d9d8a-103">Create Session</span><span class="sxs-lookup"><span data-stu-id="d9d8a-103">Create Session</span></span>

<span data-ttu-id="d9d8a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9d8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9d8a-105">Используйте этот API для создания сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-105">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="d9d8a-106">API Excel можно вызвать в одном из двух режимов:</span><span class="sxs-lookup"><span data-stu-id="d9d8a-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="d9d8a-p101">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="d9d8a-p102">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="d9d8a-113">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="d9d8a-p103">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="d9d8a-117">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="d9d8a-117">Error Handling</span></span>

<span data-ttu-id="d9d8a-118">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="d9d8a-119">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9d8a-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9d8a-120">Permissions</span></span>
<span data-ttu-id="d9d8a-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d8a-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9d8a-123">Permission type</span></span>      | <span data-ttu-id="d9d8a-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9d8a-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9d8a-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9d8a-125">Delegated (work or school account)</span></span> | <span data-ttu-id="d9d8a-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d8a-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9d8a-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9d8a-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9d8a-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-128">Not supported.</span></span>    |
|<span data-ttu-id="d9d8a-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9d8a-129">Application</span></span> | <span data-ttu-id="d9d8a-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9d8a-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9d8a-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="d9d8a-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9d8a-132">Request headers</span></span>
| <span data-ttu-id="d9d8a-133">Имя</span><span class="sxs-lookup"><span data-stu-id="d9d8a-133">Name</span></span>       | <span data-ttu-id="d9d8a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d8a-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9d8a-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9d8a-135">Authorization</span></span>  | <span data-ttu-id="d9d8a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9d8a-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9d8a-138">Request body</span></span>
<span data-ttu-id="d9d8a-139">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="d9d8a-139">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9d8a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9d8a-140">Response</span></span>

<span data-ttu-id="d9d8a-141">При успешном выполнении этот метод возвращает код ответа `201 Created` и объект [WorkbookSessionInfo](../resources/workbooksessioninfo.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-141">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9d8a-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d9d8a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9d8a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9d8a-143">Request</span></span>
<span data-ttu-id="d9d8a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9d8a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d8a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[<span data-ttu-id="d9d8a-146">C#</span><span class="sxs-lookup"><span data-stu-id="d9d8a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9d8a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9d8a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9d8a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9d8a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d9d8a-149">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="d9d8a-149">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d9d8a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9d8a-150">Response</span></span>
<span data-ttu-id="d9d8a-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9d8a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
