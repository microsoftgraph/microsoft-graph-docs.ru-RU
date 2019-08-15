---
title: Удаление домена
description: Удаление домена из клиента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec8c898c56d9c2ab4f52c0ab7075f713bb7845f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417124"
---
# <a name="delete-domain"></a><span data-ttu-id="54cb5-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="54cb5-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54cb5-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="54cb5-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="54cb5-105">**Важно!** Удаленные домены не могут быть восстановлены.</span><span class="sxs-lookup"><span data-stu-id="54cb5-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="54cb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54cb5-106">Permissions</span></span>

<span data-ttu-id="54cb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54cb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54cb5-109">Permission type</span></span>      | <span data-ttu-id="54cb5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54cb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54cb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54cb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54cb5-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54cb5-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54cb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54cb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54cb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54cb5-114">Not supported.</span></span>    |
|<span data-ttu-id="54cb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54cb5-115">Application</span></span> | <span data-ttu-id="54cb5-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54cb5-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54cb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54cb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="54cb5-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="54cb5-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54cb5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54cb5-119">Request headers</span></span>

| <span data-ttu-id="54cb5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="54cb5-120">Name</span></span>       | <span data-ttu-id="54cb5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="54cb5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="54cb5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54cb5-122">Authorization</span></span>  | <span data-ttu-id="54cb5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54cb5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54cb5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54cb5-125">Content-Type</span></span>  | <span data-ttu-id="54cb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54cb5-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="54cb5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54cb5-127">Request body</span></span>

<span data-ttu-id="54cb5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54cb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54cb5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="54cb5-129">Response</span></span>

<span data-ttu-id="54cb5-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="54cb5-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="54cb5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="54cb5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54cb5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="54cb5-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="54cb5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="54cb5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54cb5-135">C#</span><span class="sxs-lookup"><span data-stu-id="54cb5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54cb5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54cb5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54cb5-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="54cb5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="54cb5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="54cb5-138">Response</span></span>

<span data-ttu-id="54cb5-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54cb5-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
