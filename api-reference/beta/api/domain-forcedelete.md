---
title: 'домен: forceDelete'
description: Удаляет домен с помощью асинхронной операции.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47f81a25fc29f6a7eb0bb79c0f4d84e37825183a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786827"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="26164-103">домен: forceDelete</span><span class="sxs-lookup"><span data-stu-id="26164-103">domain: forceDelete</span></span>

<span data-ttu-id="26164-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26164-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26164-105">Удаляет домен с помощью асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="26164-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="26164-106">Перед [вызовом forceDelete](domain-forcedelete.md)необходимо обновить или удалить ссылки на Exchange **в** качестве службы обеспечения.</span><span class="sxs-lookup"><span data-stu-id="26164-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="26164-107">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="26164-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="26164-108">Переименование upN, EmailAddress и ProxyAddress пользователей со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="26164-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="26164-109">Переименование emailAddress групп со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="26164-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="26164-110">Переименование идентификаторов приложений со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="26164-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="26164-111">Если число объектов, которые необходимо переименовать, превышает 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="26164-111">If the number of objects to be renamed is greater than 1,000, an error is returned.</span></span>

* <span data-ttu-id="26164-112">Если одно из приложений, которое нужно переименовать, — это приложение с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="26164-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="26164-113">После завершения удаления домена операции API для удаленного домена возвращают код ответа http 404.</span><span class="sxs-lookup"><span data-stu-id="26164-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="26164-114">Чтобы убедиться в удалении домена, можно выполнить [домен get.](domain-get.md)</span><span class="sxs-lookup"><span data-stu-id="26164-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="26164-115">Если домен был успешно удален, в ответе будет возвращен код ответа http 404.</span><span class="sxs-lookup"><span data-stu-id="26164-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="26164-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26164-116">Permissions</span></span>

<span data-ttu-id="26164-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26164-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="26164-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26164-119">Permission type</span></span>      | <span data-ttu-id="26164-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26164-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26164-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26164-121">Delegated (work or school account)</span></span> | <span data-ttu-id="26164-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26164-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26164-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26164-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26164-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26164-124">Not supported.</span></span>    |
|<span data-ttu-id="26164-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="26164-125">Application</span></span> | <span data-ttu-id="26164-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26164-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26164-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26164-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="26164-128">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="26164-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26164-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26164-129">Request headers</span></span>

| <span data-ttu-id="26164-130">Имя</span><span class="sxs-lookup"><span data-stu-id="26164-130">Name</span></span>       | <span data-ttu-id="26164-131">Описание</span><span class="sxs-lookup"><span data-stu-id="26164-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26164-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26164-132">Authorization</span></span>  | <span data-ttu-id="26164-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26164-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="26164-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26164-135">Content-Type</span></span>  | <span data-ttu-id="26164-136">application/json</span><span class="sxs-lookup"><span data-stu-id="26164-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="26164-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26164-137">Request body</span></span>

<span data-ttu-id="26164-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="26164-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26164-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="26164-139">Parameter</span></span>    | <span data-ttu-id="26164-140">Тип</span><span class="sxs-lookup"><span data-stu-id="26164-140">Type</span></span>   |<span data-ttu-id="26164-141">Описание</span><span class="sxs-lookup"><span data-stu-id="26164-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26164-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="26164-142">disableUserAccounts</span></span>|<span data-ttu-id="26164-143">Логический</span><span class="sxs-lookup"><span data-stu-id="26164-143">Boolean</span></span>| <span data-ttu-id="26164-144">Параметр отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="26164-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="26164-145">Если учетная запись пользователя отключена, пользователю не будет разрешено войти.</span><span class="sxs-lookup"><span data-stu-id="26164-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="26164-146">*True* (по умолчанию) — учетные записи пользователей, переименованные в рамках этой операции, отключены.</span><span class="sxs-lookup"><span data-stu-id="26164-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="26164-147">*False* . Учетные записи пользователей, переименованные в рамках этой операции, не отключены.</span><span class="sxs-lookup"><span data-stu-id="26164-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="26164-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="26164-148">Response</span></span>

<span data-ttu-id="26164-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="26164-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="26164-150">Пример</span><span class="sxs-lookup"><span data-stu-id="26164-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="26164-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="26164-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="26164-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="26164-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="26164-153">C#</span><span class="sxs-lookup"><span data-stu-id="26164-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26164-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26164-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26164-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26164-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26164-156">Java</span><span class="sxs-lookup"><span data-stu-id="26164-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26164-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="26164-157">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


