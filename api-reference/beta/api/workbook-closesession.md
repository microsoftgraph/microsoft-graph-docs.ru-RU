---
title: Close Session
description: 'Используйте этот API для закрытия существующего сеанса книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eb6b10a5056531a58d02ab6c17186636b683435a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050292"
---
# <a name="close-session"></a><span data-ttu-id="e1ec2-103">Close Session</span><span class="sxs-lookup"><span data-stu-id="e1ec2-103">Close Session</span></span>

<span data-ttu-id="e1ec2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ec2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1ec2-105">Используйте этот API для закрытия существующего сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-105">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1ec2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1ec2-106">Permissions</span></span>
<span data-ttu-id="e1ec2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ec2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1ec2-109">Permission type</span></span>      | <span data-ttu-id="e1ec2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1ec2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1ec2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1ec2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1ec2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1ec2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1ec2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1ec2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1ec2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-114">Not supported.</span></span>    |
|<span data-ttu-id="e1ec2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1ec2-115">Application</span></span> | <span data-ttu-id="e1ec2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1ec2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1ec2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="e1ec2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1ec2-118">Request headers</span></span>
| <span data-ttu-id="e1ec2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e1ec2-119">Name</span></span>       | <span data-ttu-id="e1ec2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ec2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1ec2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1ec2-121">Authorization</span></span>  | <span data-ttu-id="e1ec2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1ec2-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="e1ec2-124">workbook-session-id</span></span> | <span data-ttu-id="e1ec2-125">Идентификатор сеанса книги, которую необходимо закрыть</span><span class="sxs-lookup"><span data-stu-id="e1ec2-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1ec2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1ec2-126">Request body</span></span>
<span data-ttu-id="e1ec2-127">Для этого API не нужно тело запроса.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="e1ec2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1ec2-128">Response</span></span>

<span data-ttu-id="e1ec2-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1ec2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e1ec2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1ec2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1ec2-131">Request</span></span>
<span data-ttu-id="e1ec2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1ec2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1ec2-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e1ec2-134">C#</span><span class="sxs-lookup"><span data-stu-id="e1ec2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1ec2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1ec2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1ec2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1ec2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e1ec2-137">Обратите внимание, что заголовок workbook-session-id является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="e1ec2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1ec2-138">Response</span></span>
<span data-ttu-id="e1ec2-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1ec2-139">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
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


