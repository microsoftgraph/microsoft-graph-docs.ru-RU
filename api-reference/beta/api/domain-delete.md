---
title: Удаление домена
description: Удаление домена из клиента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55387156e1931f851afa88ac4c33a9e100985e2a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260489"
---
# <a name="delete-domain"></a><span data-ttu-id="50a14-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="50a14-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a14-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="50a14-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="50a14-105">**Важно!** Удаленные домены не могут быть восстановлены.</span><span class="sxs-lookup"><span data-stu-id="50a14-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50a14-106">Permissions</span></span>

<span data-ttu-id="50a14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="50a14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50a14-109">Permission type</span></span>      | <span data-ttu-id="50a14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50a14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50a14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50a14-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50a14-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50a14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50a14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a14-114">Not supported.</span></span>    |
|<span data-ttu-id="50a14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50a14-115">Application</span></span> | <span data-ttu-id="50a14-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a14-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50a14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50a14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="50a14-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="50a14-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50a14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50a14-119">Request headers</span></span>

| <span data-ttu-id="50a14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="50a14-120">Name</span></span>       | <span data-ttu-id="50a14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="50a14-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50a14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50a14-122">Authorization</span></span>  | <span data-ttu-id="50a14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50a14-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50a14-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50a14-125">Content-Type</span></span>  | <span data-ttu-id="50a14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50a14-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="50a14-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50a14-127">Request body</span></span>

<span data-ttu-id="50a14-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50a14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a14-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="50a14-129">Response</span></span>

<span data-ttu-id="50a14-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="50a14-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a14-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50a14-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50a14-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="50a14-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="50a14-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="50a14-134">Response</span></span>

<span data-ttu-id="50a14-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50a14-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="50a14-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="50a14-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50a14-138">C#</span><span class="sxs-lookup"><span data-stu-id="50a14-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50a14-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="50a14-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50a14-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50a14-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
