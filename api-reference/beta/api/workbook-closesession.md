---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a75f25cb5626b523d8d8ebec01da5ee4218a2f1
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637040"
---
# <a name="close-session"></a><span data-ttu-id="4f0f9-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="4f0f9-103">Close Session</span></span>

<span data-ttu-id="4f0f9-104">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4f0f9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0f9-105">Permissions</span></span>
<span data-ttu-id="4f0f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f0f9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0f9-108">Permission type</span></span>      | <span data-ttu-id="4f0f9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f0f9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f0f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f0f9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f0f9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f0f9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f0f9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-113">Not supported.</span></span>    |
|<span data-ttu-id="4f0f9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f0f9-114">Application</span></span> | <span data-ttu-id="4f0f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f0f9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="4f0f9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f0f9-117">Request headers</span></span>
| <span data-ttu-id="4f0f9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4f0f9-118">Name</span></span>       | <span data-ttu-id="4f0f9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0f9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f0f9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f0f9-120">Authorization</span></span>  | <span data-ttu-id="4f0f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f0f9-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="4f0f9-123">workbook-session-id</span></span> | <span data-ttu-id="4f0f9-124">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="4f0f9-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f0f9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f0f9-125">Request body</span></span>
<span data-ttu-id="4f0f9-126">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="4f0f9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0f9-127">Response</span></span>

<span data-ttu-id="4f0f9-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f0f9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0f9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f0f9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0f9-130">Request</span></span>
<span data-ttu-id="4f0f9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="4f0f9-132">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="4f0f9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f0f9-133">Response</span></span>
<span data-ttu-id="4f0f9-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f0f9-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4f0f9-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="4f0f9-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="4f0f9-136">Языках</span><span class="sxs-lookup"><span data-stu-id="4f0f9-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
