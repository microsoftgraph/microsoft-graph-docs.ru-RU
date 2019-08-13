---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35f2ec6ff71e9668a7774f96acfc5ed383de076c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375319"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="b3654-103">Принудительное удаление домена</span><span class="sxs-lookup"><span data-stu-id="b3654-103">Force domain deletion</span></span>

<span data-ttu-id="b3654-104">Удаляет домен с помощью асинхронной длительной операции.</span><span class="sxs-lookup"><span data-stu-id="b3654-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="b3654-105">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="b3654-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="b3654-106">Обновляет свойства `userPrincipalName`, `mail`и `proxyAddresses` свойства `users` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b3654-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="b3654-107">Обновляет `mail` свойство `groups` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b3654-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="b3654-108">Обновляет `identifierUris` свойство `applications` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b3654-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="b3654-109">Если количество переименованных объектов больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="b3654-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="b3654-110">Если одно из `applications` наименования является приложением с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="b3654-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="b3654-111">После завершения удаления домена операции API для удаленного домена будут возвращать код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="b3654-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="b3654-112">Чтобы проверить удаление домена, можно выполнить операцию [получения домена](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="b3654-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3654-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3654-113">Permissions</span></span>

<span data-ttu-id="b3654-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3654-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3654-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3654-116">Permission type</span></span>      | <span data-ttu-id="b3654-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3654-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3654-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3654-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b3654-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3654-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3654-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3654-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3654-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3654-121">Not supported.</span></span>    |
|<span data-ttu-id="b3654-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3654-122">Application</span></span> | <span data-ttu-id="b3654-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3654-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3654-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3654-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="b3654-125">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="b3654-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3654-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3654-126">Request headers</span></span>

| <span data-ttu-id="b3654-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b3654-127">Name</span></span> | <span data-ttu-id="b3654-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b3654-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b3654-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3654-129">Authorization</span></span>  | <span data-ttu-id="b3654-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3654-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b3654-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3654-132">Content-Type</span></span>  | <span data-ttu-id="b3654-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b3654-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3654-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3654-134">Request body</span></span>

<span data-ttu-id="b3654-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b3654-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3654-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3654-136">Parameter</span></span> | <span data-ttu-id="b3654-137">Тип</span><span class="sxs-lookup"><span data-stu-id="b3654-137">Type</span></span> | <span data-ttu-id="b3654-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b3654-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="b3654-139">Параметр для отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="b3654-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="b3654-140">Если учетная запись пользователя отключена, пользователь не может войти в систему.</span><span class="sxs-lookup"><span data-stu-id="b3654-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="b3654-141">Если задано **значение true** , то `users` обновление в рамках этой операции будет отключено.</span><span class="sxs-lookup"><span data-stu-id="b3654-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="b3654-142">Значение по умолчанию: **true**.</span><span class="sxs-lookup"><span data-stu-id="b3654-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="b3654-143">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="b3654-143">Response body</span></span>

<span data-ttu-id="b3654-144">В случае успеха этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="b3654-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="b3654-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b3654-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3654-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3654-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b3654-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3654-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3654-148">C#</span><span class="sxs-lookup"><span data-stu-id="b3654-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3654-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3654-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3654-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b3654-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b3654-151">Java</span><span class="sxs-lookup"><span data-stu-id="b3654-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3654-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3654-152">Response</span></span>

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
