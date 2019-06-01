---
title: Удаление домена
description: Удаление домена из клиента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9175523580b10c6a22ac73cf88a3bc87692909f1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655798"
---
# <a name="delete-domain"></a><span data-ttu-id="53b69-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="53b69-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b69-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="53b69-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="53b69-105">**Важно!** Удаленные домены не могут быть восстановлены.</span><span class="sxs-lookup"><span data-stu-id="53b69-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b69-106">Permissions</span></span>

<span data-ttu-id="53b69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="53b69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b69-109">Permission type</span></span>      | <span data-ttu-id="53b69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53b69-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53b69-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53b69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b69-114">Not supported.</span></span>    |
|<span data-ttu-id="53b69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b69-115">Application</span></span> | <span data-ttu-id="53b69-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b69-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b69-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="53b69-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="53b69-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53b69-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b69-119">Request headers</span></span>

| <span data-ttu-id="53b69-120">Имя</span><span class="sxs-lookup"><span data-stu-id="53b69-120">Name</span></span>       | <span data-ttu-id="53b69-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53b69-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53b69-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53b69-122">Authorization</span></span>  | <span data-ttu-id="53b69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b69-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53b69-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53b69-125">Content-Type</span></span>  | <span data-ttu-id="53b69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53b69-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="53b69-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53b69-127">Request body</span></span>

<span data-ttu-id="53b69-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53b69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53b69-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="53b69-129">Response</span></span>

<span data-ttu-id="53b69-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="53b69-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b69-132">Пример</span><span class="sxs-lookup"><span data-stu-id="53b69-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53b69-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b69-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="53b69-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b69-134">Response</span></span>

<span data-ttu-id="53b69-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53b69-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="53b69-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="53b69-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53b69-138">C#</span><span class="sxs-lookup"><span data-stu-id="53b69-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53b69-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="53b69-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
