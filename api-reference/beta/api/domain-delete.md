---
title: Удаление домена
description: Удаление домена из клиента.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d6e3505ce0dc57ad29ae5dd7d440a4169e7a7c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008598"
---
# <a name="delete-domain"></a><span data-ttu-id="e67f6-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="e67f6-103">Delete domain</span></span>

<span data-ttu-id="e67f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e67f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e67f6-105">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="e67f6-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="e67f6-106">**Важно!** Удаленные домены не могут быть восстановлены.</span><span class="sxs-lookup"><span data-stu-id="e67f6-106">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="e67f6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e67f6-107">Permissions</span></span>

<span data-ttu-id="e67f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e67f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e67f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e67f6-110">Permission type</span></span>      | <span data-ttu-id="e67f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e67f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e67f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e67f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e67f6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e67f6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e67f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e67f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e67f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e67f6-115">Not supported.</span></span>    |
|<span data-ttu-id="e67f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e67f6-116">Application</span></span> | <span data-ttu-id="e67f6-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e67f6-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e67f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e67f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="e67f6-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e67f6-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e67f6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e67f6-120">Request headers</span></span>

| <span data-ttu-id="e67f6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e67f6-121">Name</span></span>       | <span data-ttu-id="e67f6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e67f6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e67f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e67f6-123">Authorization</span></span>  | <span data-ttu-id="e67f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e67f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e67f6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e67f6-126">Content-Type</span></span>  | <span data-ttu-id="e67f6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e67f6-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e67f6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e67f6-128">Request body</span></span>

<span data-ttu-id="e67f6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e67f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e67f6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e67f6-130">Response</span></span>

<span data-ttu-id="e67f6-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="e67f6-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="e67f6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e67f6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e67f6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e67f6-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e67f6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e67f6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="e67f6-136">C#</span><span class="sxs-lookup"><span data-stu-id="e67f6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e67f6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e67f6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e67f6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e67f6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e67f6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e67f6-139">Response</span></span>

<span data-ttu-id="e67f6-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e67f6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


