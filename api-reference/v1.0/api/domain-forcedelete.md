---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9219a6e49cc0c0ddc223ea1d9dd108903a21cd0
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228833"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="845eb-103">Принудительное удаление домена</span><span class="sxs-lookup"><span data-stu-id="845eb-103">Force domain deletion</span></span>

<span data-ttu-id="845eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="845eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="845eb-105">Удаляет домен с помощью асинхронной длительной операции.</span><span class="sxs-lookup"><span data-stu-id="845eb-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="845eb-106">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="845eb-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="845eb-107">Обновляет свойства `userPrincipalName`, `mail`и `proxyAddresses` свойства `users` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="845eb-107">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="845eb-108">Обновляет `mail` свойство `groups` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="845eb-108">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="845eb-109">Обновляет `identifierUris` свойство `applications` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="845eb-109">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="845eb-110">Если количество переименованных объектов больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="845eb-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="845eb-111">Если одно из `applications` наименования является приложением с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="845eb-111">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="845eb-112">После завершения удаления домена операции API для удаленного домена будут возвращать код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="845eb-112">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="845eb-113">Чтобы проверить удаление домена, можно выполнить операцию [получения домена](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="845eb-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="845eb-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="845eb-114">Permissions</span></span>

<span data-ttu-id="845eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="845eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="845eb-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="845eb-117">Permission type</span></span>      | <span data-ttu-id="845eb-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="845eb-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="845eb-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="845eb-119">Delegated (work or school account)</span></span> | <span data-ttu-id="845eb-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="845eb-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="845eb-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="845eb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="845eb-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="845eb-122">Not supported.</span></span>    |
|<span data-ttu-id="845eb-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="845eb-123">Application</span></span> | <span data-ttu-id="845eb-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="845eb-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="845eb-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="845eb-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="845eb-126">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="845eb-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="845eb-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="845eb-127">Request headers</span></span>

| <span data-ttu-id="845eb-128">Имя</span><span class="sxs-lookup"><span data-stu-id="845eb-128">Name</span></span> | <span data-ttu-id="845eb-129">Описание</span><span class="sxs-lookup"><span data-stu-id="845eb-129">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="845eb-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="845eb-130">Authorization</span></span>  | <span data-ttu-id="845eb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="845eb-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="845eb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="845eb-133">Content-Type</span></span>  | <span data-ttu-id="845eb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="845eb-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="845eb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="845eb-135">Request body</span></span>

<span data-ttu-id="845eb-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="845eb-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="845eb-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="845eb-137">Parameter</span></span> | <span data-ttu-id="845eb-138">Тип</span><span class="sxs-lookup"><span data-stu-id="845eb-138">Type</span></span> | <span data-ttu-id="845eb-139">Описание</span><span class="sxs-lookup"><span data-stu-id="845eb-139">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="845eb-140">Параметр для отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="845eb-140">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="845eb-141">Если учетная запись пользователя отключена, пользователь не может войти в систему.</span><span class="sxs-lookup"><span data-stu-id="845eb-141">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="845eb-142">Если задано **значение true** , то `users` обновление в рамках этой операции будет отключено.</span><span class="sxs-lookup"><span data-stu-id="845eb-142">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="845eb-143">Значение по умолчанию: **true**.</span><span class="sxs-lookup"><span data-stu-id="845eb-143">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="845eb-144">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="845eb-144">Response body</span></span>

<span data-ttu-id="845eb-145">В случае успеха этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="845eb-145">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="845eb-146">Пример</span><span class="sxs-lookup"><span data-stu-id="845eb-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="845eb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="845eb-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="845eb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="845eb-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="845eb-149">C#</span><span class="sxs-lookup"><span data-stu-id="845eb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="845eb-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="845eb-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="845eb-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="845eb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="845eb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="845eb-152">Response</span></span>

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
