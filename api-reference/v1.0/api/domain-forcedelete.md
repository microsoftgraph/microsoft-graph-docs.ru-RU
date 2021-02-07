---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b2e4381ee99cbd8a9e2a234328546de8b3fe4ef
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135614"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="bd30b-103">Принудительное удаление домена</span><span class="sxs-lookup"><span data-stu-id="bd30b-103">Force domain deletion</span></span>

<span data-ttu-id="bd30b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd30b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd30b-105">Удаляет домен с помощью асинхронной длительной операции.</span><span class="sxs-lookup"><span data-stu-id="bd30b-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="bd30b-106">Перед [вызовом forceDelete](domain-forcedelete.md)необходимо обновить или удалить все ссылки на **Exchange** в качестве службы предоставления.</span><span class="sxs-lookup"><span data-stu-id="bd30b-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="bd30b-107">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="bd30b-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="bd30b-108">Обновляет свойства и свойства удаленного домена, чтобы использовать исходный onmicrosoft.com `userPrincipalName` `mail` `proxyAddresses` `users` домене.</span><span class="sxs-lookup"><span data-stu-id="bd30b-108">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="bd30b-109">Обновляет свойство со ссылками на удаленный домен, чтобы использовать `mail` `groups` исходный onmicrosoft.com домена.</span><span class="sxs-lookup"><span data-stu-id="bd30b-109">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="bd30b-110">Обновляет свойство со ссылками на удаленный домен для использования `identifierUris` `applications` исходного onmicrosoft.com домена.</span><span class="sxs-lookup"><span data-stu-id="bd30b-110">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="bd30b-111">Если число объектов, которые необходимо переименовать, превышает 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="bd30b-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="bd30b-112">Если одно из `applications` переименовывуемого — мультиантийное приложение, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="bd30b-112">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="bd30b-113">После удаления домена операции API для удаленного домена возвращают код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="bd30b-113">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="bd30b-114">Чтобы проверить удаление домена, можно выполнить операцию [получения домена.](domain-get.md)</span><span class="sxs-lookup"><span data-stu-id="bd30b-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd30b-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd30b-115">Permissions</span></span>

<span data-ttu-id="bd30b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd30b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd30b-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd30b-118">Permission type</span></span>      | <span data-ttu-id="bd30b-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd30b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd30b-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd30b-120">Delegated (work or school account)</span></span> | <span data-ttu-id="bd30b-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd30b-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd30b-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd30b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd30b-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd30b-123">Not supported.</span></span>    |
|<span data-ttu-id="bd30b-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd30b-124">Application</span></span> | <span data-ttu-id="bd30b-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd30b-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd30b-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd30b-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="bd30b-127">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="bd30b-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd30b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd30b-128">Request headers</span></span>

| <span data-ttu-id="bd30b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="bd30b-129">Name</span></span> | <span data-ttu-id="bd30b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd30b-130">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bd30b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd30b-131">Authorization</span></span>  | <span data-ttu-id="bd30b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd30b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bd30b-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd30b-134">Content-Type</span></span>  | <span data-ttu-id="bd30b-135">application/json</span><span class="sxs-lookup"><span data-stu-id="bd30b-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd30b-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd30b-136">Request body</span></span>

<span data-ttu-id="bd30b-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bd30b-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd30b-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd30b-138">Parameter</span></span> | <span data-ttu-id="bd30b-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bd30b-139">Type</span></span> | <span data-ttu-id="bd30b-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bd30b-140">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="bd30b-141">Возможность отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="bd30b-141">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="bd30b-142">Если учетная запись пользователя отключена, ему не будет разрешен вход.</span><span class="sxs-lookup"><span data-stu-id="bd30b-142">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="bd30b-143">Если **установлено** `users` true, обновленное в рамках этой операции будет отключено.</span><span class="sxs-lookup"><span data-stu-id="bd30b-143">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="bd30b-144">Значение по умолчанию: **true**.</span><span class="sxs-lookup"><span data-stu-id="bd30b-144">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="bd30b-145">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="bd30b-145">Response body</span></span>

<span data-ttu-id="bd30b-146">В случае успеха этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="bd30b-146">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="bd30b-147">Пример</span><span class="sxs-lookup"><span data-stu-id="bd30b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd30b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd30b-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bd30b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd30b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="bd30b-150">C#</span><span class="sxs-lookup"><span data-stu-id="bd30b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd30b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd30b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd30b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd30b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd30b-153">Java</span><span class="sxs-lookup"><span data-stu-id="bd30b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd30b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd30b-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

