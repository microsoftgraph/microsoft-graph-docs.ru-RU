---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5983697e8685df6153cb3ad16856981b46533f17
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459841"
---
# <a name="refresh-session"></a><span data-ttu-id="d2622-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="d2622-103">Refresh Session</span></span>

<span data-ttu-id="d2622-104">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="d2622-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d2622-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2622-105">Permissions</span></span>
<span data-ttu-id="d2622-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2622-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2622-108">Permission type</span></span>      | <span data-ttu-id="d2622-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2622-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2622-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2622-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2622-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2622-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2622-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2622-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2622-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2622-113">Not supported.</span></span>    |
|<span data-ttu-id="d2622-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2622-114">Application</span></span> | <span data-ttu-id="d2622-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2622-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2622-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2622-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="d2622-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2622-117">Request headers</span></span>
| <span data-ttu-id="d2622-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d2622-118">Name</span></span>       | <span data-ttu-id="d2622-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d2622-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2622-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2622-120">Authorization</span></span>  | <span data-ttu-id="d2622-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2622-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2622-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="d2622-123">workbook-session-id</span></span> | <span data-ttu-id="d2622-124">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d2622-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2622-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2622-125">Request body</span></span>
<span data-ttu-id="d2622-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="d2622-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="d2622-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2622-127">Response</span></span>

<span data-ttu-id="d2622-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2622-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2622-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d2622-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2622-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2622-130">Request</span></span>
<span data-ttu-id="d2622-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2622-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2622-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2622-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2622-133">C#</span><span class="sxs-lookup"><span data-stu-id="d2622-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2622-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2622-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2622-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d2622-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="d2622-136">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d2622-136">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="d2622-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2622-137">Response</span></span>
<span data-ttu-id="d2622-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2622-138">Here is an example of the response.</span></span> 

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
