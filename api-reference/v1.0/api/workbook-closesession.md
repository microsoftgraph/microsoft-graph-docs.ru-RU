---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c348690e0fbe8942ddea31102adc02c08707036
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600726"
---
# <a name="close-session"></a><span data-ttu-id="e1f62-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="e1f62-103">Close Session</span></span>

<span data-ttu-id="e1f62-104">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="e1f62-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1f62-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1f62-105">Permissions</span></span>
<span data-ttu-id="e1f62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f62-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1f62-108">Permission type</span></span>      | <span data-ttu-id="e1f62-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1f62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1f62-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1f62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1f62-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1f62-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1f62-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1f62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1f62-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f62-113">Not supported.</span></span>    |
|<span data-ttu-id="e1f62-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1f62-114">Application</span></span> | <span data-ttu-id="e1f62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f62-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1f62-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1f62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="e1f62-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1f62-117">Request headers</span></span>
| <span data-ttu-id="e1f62-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e1f62-118">Name</span></span>       | <span data-ttu-id="e1f62-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f62-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1f62-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1f62-120">Authorization</span></span>  | <span data-ttu-id="e1f62-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1f62-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="e1f62-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e1f62-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e1f62-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e1f62-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="e1f62-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="e1f62-126">workbook-session-id</span></span> | <span data-ttu-id="e1f62-127">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="e1f62-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1f62-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1f62-128">Request body</span></span>
<span data-ttu-id="e1f62-129">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="e1f62-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="e1f62-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1f62-130">Response</span></span>

<span data-ttu-id="e1f62-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1f62-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1f62-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e1f62-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1f62-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1f62-133">Request</span></span>
<span data-ttu-id="e1f62-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1f62-134">Here is an example of the request.</span></span>
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

<span data-ttu-id="e1f62-135">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e1f62-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="e1f62-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1f62-136">Response</span></span>
<span data-ttu-id="e1f62-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1f62-137">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1f62-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e1f62-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1f62-139">Языках</span><span class="sxs-lookup"><span data-stu-id="e1f62-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1f62-140">Язык</span><span class="sxs-lookup"><span data-stu-id="e1f62-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/close_excel_session-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
