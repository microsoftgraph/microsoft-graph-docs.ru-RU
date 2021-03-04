---
title: Удаление orgContact
description: Удаление orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b853a153afea17bae86a7e0d4215f9ae0ac39db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434029"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="9c651-103">Удаление orgContact</span><span class="sxs-lookup"><span data-stu-id="9c651-103">Delete orgContact</span></span>

<span data-ttu-id="9c651-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c651-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c651-105">Удаление orgContact.</span><span class="sxs-lookup"><span data-stu-id="9c651-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c651-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c651-106">Permissions</span></span>
<span data-ttu-id="9c651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c651-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c651-109">Permission type</span></span>      | <span data-ttu-id="9c651-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c651-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c651-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c651-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c651-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c651-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c651-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c651-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c651-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c651-114">Not supported.</span></span>    |
|<span data-ttu-id="9c651-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c651-115">Application</span></span> | <span data-ttu-id="9c651-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c651-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c651-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c651-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9c651-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c651-118">Request headers</span></span>
| <span data-ttu-id="9c651-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9c651-119">Name</span></span>       | <span data-ttu-id="9c651-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9c651-120">Type</span></span> | <span data-ttu-id="9c651-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9c651-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c651-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c651-122">Authorization</span></span>  | <span data-ttu-id="9c651-123">string</span><span class="sxs-lookup"><span data-stu-id="9c651-123">string</span></span>  | <span data-ttu-id="9c651-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c651-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c651-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c651-126">Request body</span></span>
<span data-ttu-id="9c651-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c651-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c651-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c651-128">Response</span></span>

<span data-ttu-id="9c651-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c651-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c651-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c651-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c651-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c651-132">Request</span></span>
<span data-ttu-id="9c651-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c651-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c651-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c651-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="9c651-135">C#</span><span class="sxs-lookup"><span data-stu-id="9c651-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c651-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c651-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c651-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c651-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c651-138">Java</span><span class="sxs-lookup"><span data-stu-id="9c651-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c651-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c651-139">Response</span></span>
<span data-ttu-id="9c651-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c651-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


