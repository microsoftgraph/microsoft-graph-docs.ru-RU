---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5e4aaad295abc4ce83b8669f3d4053edafb1ad5d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575842"
---
# <a name="refresh-session"></a><span data-ttu-id="80b25-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="80b25-103">Refresh Session</span></span>

<span data-ttu-id="80b25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b25-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80b25-105">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="80b25-105">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="80b25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80b25-106">Permissions</span></span>
<span data-ttu-id="80b25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80b25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80b25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80b25-109">Permission type</span></span>      | <span data-ttu-id="80b25-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80b25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80b25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80b25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80b25-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80b25-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80b25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80b25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80b25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b25-114">Not supported.</span></span>    |
|<span data-ttu-id="80b25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80b25-115">Application</span></span> | <span data-ttu-id="80b25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b25-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80b25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80b25-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/refreshSession
POST /me/drive/root:/{item-path}:/workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="80b25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80b25-118">Request headers</span></span>
| <span data-ttu-id="80b25-119">Имя</span><span class="sxs-lookup"><span data-stu-id="80b25-119">Name</span></span>       | <span data-ttu-id="80b25-120">Описание</span><span class="sxs-lookup"><span data-stu-id="80b25-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80b25-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80b25-121">Authorization</span></span>  | <span data-ttu-id="80b25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80b25-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80b25-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="80b25-124">workbook-session-id</span></span> | <span data-ttu-id="80b25-125">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="80b25-125">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="80b25-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80b25-126">Request body</span></span>
<span data-ttu-id="80b25-127">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="80b25-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="80b25-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b25-128">Response</span></span>

<span data-ttu-id="80b25-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80b25-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80b25-130">Пример</span><span class="sxs-lookup"><span data-stu-id="80b25-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80b25-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="80b25-131">Request</span></span>
<span data-ttu-id="80b25-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80b25-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80b25-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80b25-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="c"></a>[<span data-ttu-id="80b25-134">C#</span><span class="sxs-lookup"><span data-stu-id="80b25-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80b25-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80b25-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80b25-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80b25-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80b25-137">Java</span><span class="sxs-lookup"><span data-stu-id="80b25-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="80b25-138">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="80b25-138">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="80b25-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b25-139">Response</span></span>
<span data-ttu-id="80b25-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80b25-140">Here is an example of the response.</span></span> 

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
  ]
}-->

