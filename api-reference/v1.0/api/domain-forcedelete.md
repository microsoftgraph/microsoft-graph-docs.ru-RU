---
title: Принудительно удалить домен
description: Удаление домена, с помощью асинхронной операции длительным.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 22ad640195fa9b14e0407a479438bf618d8f19c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831355"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="c8027-103">Принудительно удалить домен</span><span class="sxs-lookup"><span data-stu-id="c8027-103">Force domain deletion</span></span>

<span data-ttu-id="c8027-104">Удаление домена, с помощью асинхронной операции длительным.</span><span class="sxs-lookup"><span data-stu-id="c8027-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="c8027-105">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c8027-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="c8027-106">Обновления `userPrincipalName`, `mail`, и `proxyAddresses` свойства `users` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c8027-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c8027-107">Обновления `mail` свойства `groups` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c8027-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c8027-108">Обновления `identifierUris` свойства `applications` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c8027-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c8027-109">Если число объектов, чтобы переименовать больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="c8027-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="c8027-110">При выполнении одного из `applications` Чтобы переименовать приложения нескольких развертываний, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="c8027-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="c8027-111">После завершения удаления домена операции API для удаленного домена возвращает код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="c8027-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="c8027-112">Чтобы подтвердить удаление домена, можно выполнить операции [get домена](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="c8027-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8027-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8027-113">Permissions</span></span>

<span data-ttu-id="c8027-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8027-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8027-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8027-116">Permission type</span></span>      | <span data-ttu-id="c8027-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8027-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8027-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8027-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c8027-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8027-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8027-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8027-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8027-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8027-121">Not supported.</span></span>    |
|<span data-ttu-id="c8027-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8027-122">Application</span></span> | <span data-ttu-id="c8027-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8027-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8027-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8027-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="c8027-125">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="c8027-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8027-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8027-126">Request headers</span></span>

| <span data-ttu-id="c8027-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c8027-127">Name</span></span> | <span data-ttu-id="c8027-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c8027-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c8027-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8027-129">Authorization</span></span>  | <span data-ttu-id="c8027-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8027-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c8027-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8027-132">Content-Type</span></span>  | <span data-ttu-id="c8027-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c8027-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8027-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8027-134">Request body</span></span>

<span data-ttu-id="c8027-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c8027-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8027-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8027-136">Parameter</span></span> | <span data-ttu-id="c8027-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c8027-137">Type</span></span> | <span data-ttu-id="c8027-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c8027-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="c8027-139">Параметр, чтобы отключить учетные записи пользователей, которые были изменены при переносе.</span><span class="sxs-lookup"><span data-stu-id="c8027-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="c8027-140">Если учетная запись пользователя отключена, пользователь не разрешено вход.</span><span class="sxs-lookup"><span data-stu-id="c8027-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="c8027-141">Если задано значение **true** `users` обновлена как часть этой операции будут отключены.</span><span class="sxs-lookup"><span data-stu-id="c8027-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="c8027-142">Значение по умолчанию — **true**.</span><span class="sxs-lookup"><span data-stu-id="c8027-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="c8027-143">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="c8027-143">Response body</span></span>

<span data-ttu-id="c8027-144">Успешно завершена, этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="c8027-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="c8027-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c8027-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8027-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8027-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="c8027-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8027-147">Response</span></span>

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
  "tocPath": ""
}-->
