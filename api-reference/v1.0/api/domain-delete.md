---
title: Удаление домена
description: Удаление домена из клиента.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0ecaf2cd5c1f8f0ed0281be585a85008e6870a8f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050509"
---
# <a name="delete-domain"></a><span data-ttu-id="e3be5-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="e3be5-103">Delete domain</span></span>

<span data-ttu-id="e3be5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3be5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3be5-105">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="e3be5-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="e3be5-106">**Важно!**</span><span class="sxs-lookup"><span data-stu-id="e3be5-106">**Important:**</span></span>
> - <span data-ttu-id="e3be5-107">Вам не удастся восстановить удаленные домены.</span><span class="sxs-lookup"><span data-stu-id="e3be5-107">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="e3be5-p101">Вам не удастся удалить домен, если какие-либо ресурсы или объекты все еще зависят от него. Вы можете найти все зависимые ресурсы с помощью API [перечисления domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="e3be5-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3be5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3be5-110">Permissions</span></span>

<span data-ttu-id="e3be5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3be5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e3be5-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3be5-113">Permission type</span></span>      | <span data-ttu-id="e3be5-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3be5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3be5-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3be5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e3be5-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3be5-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3be5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3be5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3be5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3be5-118">Not supported.</span></span>    |
|<span data-ttu-id="e3be5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3be5-119">Application</span></span> | <span data-ttu-id="e3be5-120">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3be5-120">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3be5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3be5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="e3be5-122">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e3be5-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3be5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3be5-123">Request headers</span></span>

| <span data-ttu-id="e3be5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e3be5-124">Name</span></span>       | <span data-ttu-id="e3be5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e3be5-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e3be5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3be5-126">Authorization</span></span>  | <span data-ttu-id="e3be5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3be5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3be5-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3be5-129">Content-Type</span></span>  | <span data-ttu-id="e3be5-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e3be5-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3be5-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3be5-131">Request body</span></span>

<span data-ttu-id="e3be5-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3be5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3be5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3be5-133">Response</span></span>

<span data-ttu-id="e3be5-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="e3be5-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3be5-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e3be5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3be5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3be5-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e3be5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3be5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="e3be5-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3be5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3be5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3be5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3be5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3be5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3be5-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3be5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3be5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3be5-143">Response</span></span>

<span data-ttu-id="e3be5-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3be5-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

