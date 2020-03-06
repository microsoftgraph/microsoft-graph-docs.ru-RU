---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ee16d09d61df2f805d7af50748935a588e578c1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508886"
---
# <a name="close-session"></a><span data-ttu-id="ad3b0-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="ad3b0-103">Close Session</span></span>

<span data-ttu-id="ad3b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad3b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad3b0-105">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-105">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ad3b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad3b0-106">Permissions</span></span>
<span data-ttu-id="ad3b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad3b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad3b0-109">Permission type</span></span>      | <span data-ttu-id="ad3b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad3b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad3b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad3b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad3b0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad3b0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad3b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad3b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad3b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-114">Not supported.</span></span>    |
|<span data-ttu-id="ad3b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad3b0-115">Application</span></span> | <span data-ttu-id="ad3b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad3b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad3b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="ad3b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad3b0-118">Request headers</span></span>
| <span data-ttu-id="ad3b0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ad3b0-119">Name</span></span>       | <span data-ttu-id="ad3b0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad3b0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad3b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad3b0-121">Authorization</span></span>  | <span data-ttu-id="ad3b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="ad3b0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ad3b0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ad3b0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="ad3b0-127">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="ad3b0-127">workbook-session-id</span></span> | <span data-ttu-id="ad3b0-128">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="ad3b0-128">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad3b0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad3b0-129">Request body</span></span>
<span data-ttu-id="ad3b0-130">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-130">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="ad3b0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad3b0-131">Response</span></span>

<span data-ttu-id="ad3b0-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad3b0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ad3b0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad3b0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad3b0-134">Request</span></span>
<span data-ttu-id="ad3b0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad3b0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad3b0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="c"></a>[<span data-ttu-id="ad3b0-137">C#</span><span class="sxs-lookup"><span data-stu-id="ad3b0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad3b0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad3b0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad3b0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad3b0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad3b0-140">Java</span><span class="sxs-lookup"><span data-stu-id="ad3b0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ad3b0-141">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-141">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="ad3b0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad3b0-142">Response</span></span>
<span data-ttu-id="ad3b0-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad3b0-143">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
