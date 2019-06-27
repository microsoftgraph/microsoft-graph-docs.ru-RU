---
title: Refresh Session
description: 'Используйте этот API для обновления существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f5519d447c8e752a000ee8b260a383fb586cd7be
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278584"
---
# <a name="refresh-session"></a><span data-ttu-id="27896-103">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="27896-103">Refresh Session</span></span>

<span data-ttu-id="27896-104">Используйте этот API для обновления существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="27896-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="27896-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27896-105">Permissions</span></span>
<span data-ttu-id="27896-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27896-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27896-108">Permission type</span></span>      | <span data-ttu-id="27896-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27896-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27896-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27896-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27896-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27896-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="27896-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27896-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27896-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27896-113">Not supported.</span></span>    |
|<span data-ttu-id="27896-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27896-114">Application</span></span> | <span data-ttu-id="27896-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27896-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27896-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27896-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="27896-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27896-117">Request headers</span></span>
| <span data-ttu-id="27896-118">Имя</span><span class="sxs-lookup"><span data-stu-id="27896-118">Name</span></span>       | <span data-ttu-id="27896-119">Описание</span><span class="sxs-lookup"><span data-stu-id="27896-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27896-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27896-120">Authorization</span></span>  | <span data-ttu-id="27896-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27896-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27896-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="27896-123">workbook-session-id</span></span> | <span data-ttu-id="27896-124">Идентификатор сеанса для книги, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="27896-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="27896-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27896-125">Request body</span></span>
<span data-ttu-id="27896-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="27896-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="27896-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="27896-127">Response</span></span>

<span data-ttu-id="27896-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27896-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27896-129">Пример</span><span class="sxs-lookup"><span data-stu-id="27896-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27896-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="27896-130">Request</span></span>
<span data-ttu-id="27896-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27896-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="27896-132">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="27896-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="27896-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="27896-133">Response</span></span>
<span data-ttu-id="27896-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27896-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27896-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="27896-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27896-136">C#</span><span class="sxs-lookup"><span data-stu-id="27896-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27896-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="27896-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="27896-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="27896-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
