---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 884dc0355f7afc8e9e86a59a73101d33d7250166
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026441"
---
# <a name="refresh-session"></a><span data-ttu-id="3b557-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="3b557-103">Refresh Session</span></span>

<span data-ttu-id="3b557-104">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="3b557-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3b557-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b557-105">Permissions</span></span>
<span data-ttu-id="3b557-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b557-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b557-108">Permission type</span></span>      | <span data-ttu-id="3b557-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b557-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b557-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b557-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b557-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b557-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b557-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b557-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b557-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b557-113">Not supported.</span></span>    |
|<span data-ttu-id="3b557-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b557-114">Application</span></span> | <span data-ttu-id="3b557-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b557-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b557-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b557-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="3b557-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b557-117">Request headers</span></span>
| <span data-ttu-id="3b557-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3b557-118">Name</span></span>       | <span data-ttu-id="3b557-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3b557-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b557-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b557-120">Authorization</span></span>  | <span data-ttu-id="3b557-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b557-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b557-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="3b557-123">workbook-session-id</span></span> | <span data-ttu-id="3b557-124">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3b557-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b557-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b557-125">Request body</span></span>
<span data-ttu-id="3b557-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="3b557-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="3b557-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b557-127">Response</span></span>

<span data-ttu-id="3b557-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b557-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b557-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3b557-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b557-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b557-130">Request</span></span>
<span data-ttu-id="3b557-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b557-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3b557-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b557-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b557-133">C#</span><span class="sxs-lookup"><span data-stu-id="3b557-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b557-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3b557-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b557-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3b557-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3b557-136">Java</span><span class="sxs-lookup"><span data-stu-id="3b557-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3b557-137">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="3b557-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="3b557-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b557-138">Response</span></span>
<span data-ttu-id="3b557-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b557-139">Here is an example of the response.</span></span> 

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
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
