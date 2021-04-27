---
title: Удаление домена
description: Удаление домена из клиента.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5f00627823d4a9cc571143c8e0e09ba297bd4902
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046540"
---
# <a name="delete-domain"></a><span data-ttu-id="88136-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="88136-103">Delete domain</span></span>

<span data-ttu-id="88136-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88136-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88136-105">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="88136-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="88136-106">**Важно:** Удаленные домены не могут быть восстановлены.</span><span class="sxs-lookup"><span data-stu-id="88136-106">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="88136-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88136-107">Permissions</span></span>

<span data-ttu-id="88136-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88136-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88136-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88136-110">Permission type</span></span>      | <span data-ttu-id="88136-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88136-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88136-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88136-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88136-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88136-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88136-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88136-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88136-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88136-115">Not supported.</span></span>    |
|<span data-ttu-id="88136-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88136-116">Application</span></span> | <span data-ttu-id="88136-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88136-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88136-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88136-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="88136-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="88136-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88136-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88136-120">Request headers</span></span>

| <span data-ttu-id="88136-121">Имя</span><span class="sxs-lookup"><span data-stu-id="88136-121">Name</span></span>       | <span data-ttu-id="88136-122">Описание</span><span class="sxs-lookup"><span data-stu-id="88136-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88136-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88136-123">Authorization</span></span>  | <span data-ttu-id="88136-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88136-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88136-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88136-126">Content-Type</span></span>  | <span data-ttu-id="88136-127">application/json</span><span class="sxs-lookup"><span data-stu-id="88136-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="88136-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88136-128">Request body</span></span>

<span data-ttu-id="88136-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88136-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88136-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="88136-130">Response</span></span>

<span data-ttu-id="88136-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="88136-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="88136-133">Пример</span><span class="sxs-lookup"><span data-stu-id="88136-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88136-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="88136-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88136-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="88136-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="88136-136">C#</span><span class="sxs-lookup"><span data-stu-id="88136-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88136-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88136-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88136-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88136-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88136-139">Java</span><span class="sxs-lookup"><span data-stu-id="88136-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88136-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88136-140">Response</span></span>

<span data-ttu-id="88136-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88136-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


