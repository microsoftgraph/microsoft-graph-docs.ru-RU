---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 645526a659dc7099067364cb0a7dd6d68584dec1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972908"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="9cf4c-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="9cf4c-103">Delete Outlook category</span></span>

<span data-ttu-id="9cf4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf4c-105">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="9cf4c-105">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cf4c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cf4c-106">Permissions</span></span>
<span data-ttu-id="9cf4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf4c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cf4c-109">Permission type</span></span>      | <span data-ttu-id="9cf4c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cf4c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cf4c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cf4c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9cf4c-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf4c-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9cf4c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cf4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf4c-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf4c-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9cf4c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cf4c-115">Application</span></span> | <span data-ttu-id="9cf4c-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf4c-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cf4c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cf4c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9cf4c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cf4c-118">Request headers</span></span>
| <span data-ttu-id="9cf4c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9cf4c-119">Name</span></span>      |<span data-ttu-id="9cf4c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9cf4c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cf4c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cf4c-121">Authorization</span></span>  | <span data-ttu-id="9cf4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cf4c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cf4c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cf4c-124">Request body</span></span>
<span data-ttu-id="9cf4c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cf4c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cf4c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cf4c-126">Response</span></span>

<span data-ttu-id="9cf4c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9cf4c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf4c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9cf4c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cf4c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cf4c-130">Request</span></span>
<span data-ttu-id="9cf4c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cf4c-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cf4c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf4c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="c"></a>[<span data-ttu-id="9cf4c-133">C#</span><span class="sxs-lookup"><span data-stu-id="9cf4c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cf4c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf4c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cf4c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf4c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cf4c-136">Java</span><span class="sxs-lookup"><span data-stu-id="9cf4c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cf4c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cf4c-137">Response</span></span>
<span data-ttu-id="9cf4c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9cf4c-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


