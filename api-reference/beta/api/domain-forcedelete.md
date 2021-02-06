---
title: 'domain: forceDelete'
description: Удаляет домен с помощью асинхронной операции.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc074f3160ef8260f04fe2795a58a0ddfd1c54d7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131273"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="1d0f6-103">domain: forceDelete</span><span class="sxs-lookup"><span data-stu-id="1d0f6-103">domain: forceDelete</span></span>

<span data-ttu-id="1d0f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d0f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d0f6-105">Удаляет домен с помощью асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="1d0f6-106">Перед [вызовом forceDelete](domain-forcedelete.md)необходимо обновить или удалить все ссылки на **Exchange** в качестве службы предоставления.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="1d0f6-107">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1d0f6-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="1d0f6-108">Переименовывая имя пользователя, адрес emailAddress и ProxyAddress пользователей, ссылаясь на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="1d0f6-109">Переименовка Адреса электронной почты групп со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="1d0f6-110">Переименовывая идентификаторы приложений со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="1d0f6-111">Если число объектов, которые необходимо переименовать, превышает 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-111">If the number of objects to be renamed is greater than 1,000, an error is returned.</span></span>

* <span data-ttu-id="1d0f6-112">Если одно из приложений, которые необходимо переименовать, — мультиязычное, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="1d0f6-113">После удаления домена операции API для удаленного домена возвращают код отклика HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="1d0f6-114">Чтобы проверить удаление домена, можно выполнить получить [домен.](domain-get.md)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="1d0f6-115">Если домен был успешно удален, в ответе будет возвращен код http-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d0f6-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d0f6-116">Permissions</span></span>

<span data-ttu-id="1d0f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d0f6-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d0f6-119">Permission type</span></span>      | <span data-ttu-id="1d0f6-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d0f6-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1d0f6-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d0f6-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d0f6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d0f6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d0f6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-124">Not supported.</span></span>    |
|<span data-ttu-id="1d0f6-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d0f6-125">Application</span></span> | <span data-ttu-id="1d0f6-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0f6-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d0f6-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d0f6-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="1d0f6-128">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d0f6-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d0f6-129">Request headers</span></span>

| <span data-ttu-id="1d0f6-130">Имя</span><span class="sxs-lookup"><span data-stu-id="1d0f6-130">Name</span></span>       | <span data-ttu-id="1d0f6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1d0f6-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d0f6-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d0f6-132">Authorization</span></span>  | <span data-ttu-id="1d0f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1d0f6-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d0f6-135">Content-Type</span></span>  | <span data-ttu-id="1d0f6-136">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0f6-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d0f6-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d0f6-137">Request body</span></span>

<span data-ttu-id="1d0f6-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d0f6-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="1d0f6-139">Parameter</span></span>    | <span data-ttu-id="1d0f6-140">Тип</span><span class="sxs-lookup"><span data-stu-id="1d0f6-140">Type</span></span>   |<span data-ttu-id="1d0f6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1d0f6-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d0f6-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="1d0f6-142">disableUserAccounts</span></span>|<span data-ttu-id="1d0f6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d0f6-143">Boolean</span></span>| <span data-ttu-id="1d0f6-144">Возможность отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="1d0f6-145">Если учетная запись пользователя отключена, ему не будет разрешен вход.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="1d0f6-146">*True* (по умолчанию) — учетные записи пользователей, переименованные в рамках этой операции, отключены.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="1d0f6-147">*False* — учетные записи пользователей, переименованные в рамках этой операции, не отключены.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="1d0f6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d0f6-148">Response</span></span>

<span data-ttu-id="1d0f6-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1d0f6-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="1d0f6-150">Пример</span><span class="sxs-lookup"><span data-stu-id="1d0f6-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d0f6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d0f6-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1d0f6-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0f6-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1d0f6-153">C#</span><span class="sxs-lookup"><span data-stu-id="1d0f6-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d0f6-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d0f6-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d0f6-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d0f6-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d0f6-156">Java</span><span class="sxs-lookup"><span data-stu-id="1d0f6-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d0f6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d0f6-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


