---
title: Удаление домена
description: Удаление домена из клиента.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 03bc5e121d8ef3c6c0271db206849376e0764899
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181352"
---
# <a name="delete-domain"></a><span data-ttu-id="5fb41-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="5fb41-103">Delete domain</span></span>

<span data-ttu-id="5fb41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fb41-105">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="5fb41-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="5fb41-106">**Важно!**</span><span class="sxs-lookup"><span data-stu-id="5fb41-106">**Important:**</span></span>
> - <span data-ttu-id="5fb41-107">Вам не удастся восстановить удаленные домены.</span><span class="sxs-lookup"><span data-stu-id="5fb41-107">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="5fb41-p101">Вам не удастся удалить домен, если какие-либо ресурсы или объекты все еще зависят от него. Вы можете найти все зависимые ресурсы с помощью API [перечисления domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="5fb41-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fb41-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb41-110">Permissions</span></span>

<span data-ttu-id="5fb41-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fb41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5fb41-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fb41-113">Permission type</span></span>      | <span data-ttu-id="5fb41-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fb41-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fb41-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fb41-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5fb41-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5fb41-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5fb41-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fb41-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fb41-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fb41-118">Not supported.</span></span>    |
|<span data-ttu-id="5fb41-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fb41-119">Application</span></span> | <span data-ttu-id="5fb41-120">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb41-120">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fb41-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fb41-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="5fb41-122">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="5fb41-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fb41-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fb41-123">Request headers</span></span>

| <span data-ttu-id="5fb41-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5fb41-124">Name</span></span>       | <span data-ttu-id="5fb41-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb41-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5fb41-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fb41-126">Authorization</span></span>  | <span data-ttu-id="5fb41-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fb41-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fb41-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5fb41-129">Content-Type</span></span>  | <span data-ttu-id="5fb41-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5fb41-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fb41-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fb41-131">Request body</span></span>

<span data-ttu-id="5fb41-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5fb41-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fb41-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5fb41-133">Response</span></span>

<span data-ttu-id="5fb41-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="5fb41-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb41-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5fb41-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fb41-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fb41-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5fb41-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fb41-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="5fb41-139">C#</span><span class="sxs-lookup"><span data-stu-id="5fb41-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fb41-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fb41-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fb41-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fb41-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fb41-142">Java</span><span class="sxs-lookup"><span data-stu-id="5fb41-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5fb41-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fb41-143">Response</span></span>

<span data-ttu-id="5fb41-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5fb41-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
