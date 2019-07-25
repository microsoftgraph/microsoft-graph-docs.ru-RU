---
title: Удаление домена
description: Удаление домена из клиента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: efef594979cecc17f740d6be683ad08f091bdf71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889980"
---
# <a name="delete-domain"></a><span data-ttu-id="821b1-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="821b1-103">Delete domain</span></span>

<span data-ttu-id="821b1-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="821b1-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="821b1-105">**Важно!**</span><span class="sxs-lookup"><span data-stu-id="821b1-105">**Important:**</span></span>
> - <span data-ttu-id="821b1-106">Вам не удастся восстановить удаленные домены.</span><span class="sxs-lookup"><span data-stu-id="821b1-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="821b1-p101">Вам не удастся удалить домен, если какие-либо ресурсы или объекты все еще зависят от него. Вы можете найти все зависимые ресурсы с помощью API [перечисления domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="821b1-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="821b1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="821b1-109">Permissions</span></span>

<span data-ttu-id="821b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="821b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="821b1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="821b1-112">Permission type</span></span>      | <span data-ttu-id="821b1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="821b1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="821b1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="821b1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="821b1-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="821b1-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="821b1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="821b1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="821b1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="821b1-117">Not supported.</span></span>    |
|<span data-ttu-id="821b1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="821b1-118">Application</span></span> | <span data-ttu-id="821b1-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="821b1-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="821b1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="821b1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="821b1-121">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="821b1-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="821b1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="821b1-122">Request headers</span></span>

| <span data-ttu-id="821b1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="821b1-123">Name</span></span>       | <span data-ttu-id="821b1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="821b1-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="821b1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="821b1-125">Authorization</span></span>  | <span data-ttu-id="821b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="821b1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="821b1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="821b1-128">Content-Type</span></span>  | <span data-ttu-id="821b1-129">application/json</span><span class="sxs-lookup"><span data-stu-id="821b1-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="821b1-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="821b1-130">Request body</span></span>

<span data-ttu-id="821b1-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="821b1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="821b1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="821b1-132">Response</span></span>

<span data-ttu-id="821b1-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="821b1-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="821b1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="821b1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="821b1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="821b1-136">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="821b1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="821b1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="821b1-138">C#</span><span class="sxs-lookup"><span data-stu-id="821b1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="821b1-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="821b1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="821b1-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="821b1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="821b1-141">Java</span><span class="sxs-lookup"><span data-stu-id="821b1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="821b1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="821b1-142">Response</span></span>

<span data-ttu-id="821b1-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="821b1-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
