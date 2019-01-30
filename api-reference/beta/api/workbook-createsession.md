---
title: Create Session
description: 'Используйте этот API для создания сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ab4cc0d983efde535a4d92b6e918dfe9c9881170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641864"
---
# <a name="create-session"></a><span data-ttu-id="c71a8-103">Create Session</span><span class="sxs-lookup"><span data-stu-id="c71a8-103">Create Session</span></span>

<span data-ttu-id="c71a8-104">Используйте этот API для создания сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="c71a8-104">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="c71a8-105">API Excel можно вызвать в одном из двух режимов:</span><span class="sxs-lookup"><span data-stu-id="c71a8-105">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="c71a8-p101">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="c71a8-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="c71a8-p102">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="c71a8-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="c71a8-112">Чтобы представить сеанс в API, воспользуйтесь заголовком `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="c71a8-112">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="c71a8-p103">**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.</span><span class="sxs-lookup"><span data-stu-id="c71a8-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="c71a8-116">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="c71a8-116">Error Handling</span></span>

<span data-ttu-id="c71a8-117">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="c71a8-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="c71a8-118">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="c71a8-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c71a8-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c71a8-119">Permissions</span></span>
<span data-ttu-id="c71a8-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c71a8-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c71a8-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c71a8-122">Permission type</span></span>      | <span data-ttu-id="c71a8-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c71a8-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c71a8-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c71a8-124">Delegated (work or school account)</span></span> | <span data-ttu-id="c71a8-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c71a8-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c71a8-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c71a8-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c71a8-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c71a8-127">Not supported.</span></span>    |
|<span data-ttu-id="c71a8-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c71a8-128">Application</span></span> | <span data-ttu-id="c71a8-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c71a8-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c71a8-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c71a8-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="c71a8-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c71a8-131">Request headers</span></span>
| <span data-ttu-id="c71a8-132">Имя</span><span class="sxs-lookup"><span data-stu-id="c71a8-132">Name</span></span>       | <span data-ttu-id="c71a8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c71a8-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c71a8-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c71a8-134">Authorization</span></span>  | <span data-ttu-id="c71a8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c71a8-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c71a8-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c71a8-137">Request body</span></span>
<span data-ttu-id="c71a8-138">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="c71a8-138">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c71a8-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c71a8-139">Response</span></span>

<span data-ttu-id="c71a8-140">При успешном выполнении этот метод возвращает код ответа `201 Created` и объект [WorkbookSessionInfo](../resources/workbooksessioninfo.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c71a8-140">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c71a8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c71a8-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c71a8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c71a8-142">Request</span></span>
<span data-ttu-id="c71a8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c71a8-143">Here is an example of the request.</span></span>
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
<span data-ttu-id="c71a8-144">В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="c71a8-144">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c71a8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="c71a8-145">Response</span></span>
<span data-ttu-id="c71a8-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c71a8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

