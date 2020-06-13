---
title: Create Session
description: 'Используйте этот API для создания сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 86324352e70938fc0a29cec2aa3398141dd59ac5
ms.sourcegitcommit: d6374f42bee4de11fd7a3d0d8c2a7f8c4e7739bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2020
ms.locfileid: "44710617"
---
# <a name="create-session"></a><span data-ttu-id="48789-103">Create Session</span><span class="sxs-lookup"><span data-stu-id="48789-103">Create Session</span></span>

<span data-ttu-id="48789-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48789-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48789-105">Используйте этот API для создания сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="48789-105">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="48789-106">API Excel можно вызвать в одном из двух режимов:</span><span class="sxs-lookup"><span data-stu-id="48789-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="48789-p101">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="48789-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="48789-p102">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="48789-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="48789-113">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="48789-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="48789-p103">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="48789-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="48789-117">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="48789-117">Error Handling</span></span>

<span data-ttu-id="48789-118">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="48789-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="48789-119">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="48789-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="48789-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48789-120">Permissions</span></span>
<span data-ttu-id="48789-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48789-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48789-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48789-123">Permission type</span></span>      | <span data-ttu-id="48789-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48789-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48789-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48789-125">Delegated (work or school account)</span></span> | <span data-ttu-id="48789-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48789-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48789-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48789-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48789-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48789-128">Not supported.</span></span>    |
|<span data-ttu-id="48789-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48789-129">Application</span></span> | <span data-ttu-id="48789-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48789-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48789-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48789-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession
```
## <a name="request-headers"></a><span data-ttu-id="48789-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48789-132">Request headers</span></span>
| <span data-ttu-id="48789-133">Имя</span><span class="sxs-lookup"><span data-stu-id="48789-133">Name</span></span>       | <span data-ttu-id="48789-134">Описание</span><span class="sxs-lookup"><span data-stu-id="48789-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48789-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48789-135">Authorization</span></span>  | <span data-ttu-id="48789-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48789-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48789-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48789-138">Request body</span></span>
<span data-ttu-id="48789-139">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="48789-139">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48789-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="48789-140">Response</span></span>

<span data-ttu-id="48789-141">При успешном выполнении этот метод возвращает код ответа `201 Created` и объект [WorkbookSessionInfo](../resources/workbooksessioninfo.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48789-141">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48789-142">Пример</span><span class="sxs-lookup"><span data-stu-id="48789-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48789-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="48789-143">Request</span></span>
<span data-ttu-id="48789-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48789-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48789-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="48789-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="48789-146">C#</span><span class="sxs-lookup"><span data-stu-id="48789-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48789-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48789-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48789-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48789-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48789-149">Java</span><span class="sxs-lookup"><span data-stu-id="48789-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="48789-150">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="48789-150">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="48789-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="48789-151">Response</span></span>
<span data-ttu-id="48789-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48789-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
