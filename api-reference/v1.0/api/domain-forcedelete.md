---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a4376961ea843c5c512d5bdf59449a7e765399f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441979"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="648ca-103">Принудительное удаление домена</span><span class="sxs-lookup"><span data-stu-id="648ca-103">Force domain deletion</span></span>

<span data-ttu-id="648ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="648ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="648ca-105">Удаляет домен с помощью асинхронной длительной операции.</span><span class="sxs-lookup"><span data-stu-id="648ca-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="648ca-106">Перед [вызовом forceDelete](domain-forcedelete.md)необходимо обновить или удалить ссылки на **Exchange** в качестве службы подготовка.</span><span class="sxs-lookup"><span data-stu-id="648ca-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="648ca-107">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="648ca-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="648ca-108">Обновляет свойства и свойства домена со ссылками на удаленный домен для использования исходного onmicrosoft.com `userPrincipalName` `mail` `proxyAddresses` `users` домена.</span><span class="sxs-lookup"><span data-stu-id="648ca-108">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="648ca-109">Обновляет свойство со ссылками на удаленный домен для использования исходного onmicrosoft.com `mail` `groups` домена.</span><span class="sxs-lookup"><span data-stu-id="648ca-109">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="648ca-110">Обновляет свойство со ссылками на удаленный домен для использования исходного onmicrosoft.com `identifierUris` `applications` домена.</span><span class="sxs-lookup"><span data-stu-id="648ca-110">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="648ca-111">Если число объектов, которые будут переименованы, превышает 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="648ca-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="648ca-112">Если одно из переименованных — это приложение с несколькими `applications` клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="648ca-112">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="648ca-113">После завершения удаления домена операции API для удаленного домена возвращают код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="648ca-113">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="648ca-114">Чтобы проверить удаление домена, можно выполнить операцию [получения домена.](domain-get.md)</span><span class="sxs-lookup"><span data-stu-id="648ca-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="648ca-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="648ca-115">Permissions</span></span>

<span data-ttu-id="648ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="648ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="648ca-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="648ca-118">Permission type</span></span>      | <span data-ttu-id="648ca-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="648ca-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="648ca-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="648ca-120">Delegated (work or school account)</span></span> | <span data-ttu-id="648ca-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="648ca-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="648ca-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="648ca-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="648ca-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="648ca-123">Not supported.</span></span>    |
|<span data-ttu-id="648ca-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="648ca-124">Application</span></span> | <span data-ttu-id="648ca-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="648ca-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="648ca-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="648ca-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="648ca-127">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="648ca-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="648ca-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="648ca-128">Request headers</span></span>

| <span data-ttu-id="648ca-129">Имя</span><span class="sxs-lookup"><span data-stu-id="648ca-129">Name</span></span> | <span data-ttu-id="648ca-130">Описание</span><span class="sxs-lookup"><span data-stu-id="648ca-130">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="648ca-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="648ca-131">Authorization</span></span>  | <span data-ttu-id="648ca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="648ca-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="648ca-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="648ca-134">Content-Type</span></span>  | <span data-ttu-id="648ca-135">application/json</span><span class="sxs-lookup"><span data-stu-id="648ca-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="648ca-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="648ca-136">Request body</span></span>

<span data-ttu-id="648ca-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="648ca-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="648ca-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="648ca-138">Parameter</span></span> | <span data-ttu-id="648ca-139">Тип</span><span class="sxs-lookup"><span data-stu-id="648ca-139">Type</span></span> | <span data-ttu-id="648ca-140">Описание</span><span class="sxs-lookup"><span data-stu-id="648ca-140">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="648ca-141">Параметр отключения учетных записей пользователей, которые переименованы.</span><span class="sxs-lookup"><span data-stu-id="648ca-141">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="648ca-142">Если учетная запись пользователя отключена, пользователю не будет разрешено войти.</span><span class="sxs-lookup"><span data-stu-id="648ca-142">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="648ca-143">Если **установлено,** что обновленная версия в рамках этой операции `users` будет отключена.</span><span class="sxs-lookup"><span data-stu-id="648ca-143">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="648ca-144">Значение по умолчанию: **true**.</span><span class="sxs-lookup"><span data-stu-id="648ca-144">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="648ca-145">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="648ca-145">Response body</span></span>

<span data-ttu-id="648ca-146">В случае успешной работы этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="648ca-146">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="648ca-147">Пример</span><span class="sxs-lookup"><span data-stu-id="648ca-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="648ca-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="648ca-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="648ca-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="648ca-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="648ca-150">C#</span><span class="sxs-lookup"><span data-stu-id="648ca-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="648ca-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="648ca-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="648ca-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="648ca-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="648ca-153">Java</span><span class="sxs-lookup"><span data-stu-id="648ca-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="648ca-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="648ca-154">Response</span></span>

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

