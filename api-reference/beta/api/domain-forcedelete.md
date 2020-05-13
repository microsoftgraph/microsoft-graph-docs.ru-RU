---
title: 'домен: Форцеделете'
description: Удаляет домен, используя асинхронную операцию.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4daff04db42782a5d9b611d454a5cfb2c12953b1
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43180104"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="b49d2-103">домен: Форцеделете</span><span class="sxs-lookup"><span data-stu-id="b49d2-103">domain: forceDelete</span></span>

<span data-ttu-id="b49d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b49d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b49d2-105">Удаляет домен, используя асинхронную операцию.</span><span class="sxs-lookup"><span data-stu-id="b49d2-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="b49d2-106">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="b49d2-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="b49d2-107">Переименовывает имя участника-пользователя, EmailAddress и ProxyAddress пользователей со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="b49d2-107">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="b49d2-108">Переименование EmailAddress групп со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="b49d2-108">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="b49d2-109">Переименовывает С identifieruris приложений со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="b49d2-109">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="b49d2-110">Если количество переименованных объектов больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="b49d2-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="b49d2-111">Если одно из переименованных приложений является приложением с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="b49d2-111">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="b49d2-112">После завершения удаления домена операции API для удаленного домена будут возвращать код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="b49d2-112">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="b49d2-113">Чтобы проверить удаление домена, можно выполнить [Получение домена](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="b49d2-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="b49d2-114">Если домен был успешно удален, в ответе будет возвращен код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="b49d2-114">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="b49d2-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b49d2-115">Permissions</span></span>

<span data-ttu-id="b49d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b49d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b49d2-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b49d2-118">Permission type</span></span>      | <span data-ttu-id="b49d2-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b49d2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b49d2-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b49d2-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b49d2-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b49d2-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b49d2-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b49d2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b49d2-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b49d2-123">Not supported.</span></span>    |
|<span data-ttu-id="b49d2-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b49d2-124">Application</span></span> | <span data-ttu-id="b49d2-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49d2-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b49d2-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b49d2-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="b49d2-127">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="b49d2-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b49d2-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b49d2-128">Request headers</span></span>

| <span data-ttu-id="b49d2-129">Имя</span><span class="sxs-lookup"><span data-stu-id="b49d2-129">Name</span></span>       | <span data-ttu-id="b49d2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b49d2-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b49d2-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b49d2-131">Authorization</span></span>  | <span data-ttu-id="b49d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b49d2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b49d2-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b49d2-134">Content-Type</span></span>  | <span data-ttu-id="b49d2-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b49d2-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b49d2-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b49d2-136">Request body</span></span>

<span data-ttu-id="b49d2-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b49d2-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b49d2-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="b49d2-138">Parameter</span></span>    | <span data-ttu-id="b49d2-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b49d2-139">Type</span></span>   |<span data-ttu-id="b49d2-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b49d2-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b49d2-141">дисаблеусераккаунтс</span><span class="sxs-lookup"><span data-stu-id="b49d2-141">disableUserAccounts</span></span>|<span data-ttu-id="b49d2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b49d2-142">Boolean</span></span>| <span data-ttu-id="b49d2-143">Возможность отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="b49d2-143">Option to disable renamed user accounts.</span></span> <span data-ttu-id="b49d2-144">Если учетная запись пользователя отключена, пользователь не может войти в систему.</span><span class="sxs-lookup"><span data-stu-id="b49d2-144">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="b49d2-145">*True* (по умолчанию) — учетные записи пользователей, переименованные в рамках этой операции, отключены.</span><span class="sxs-lookup"><span data-stu-id="b49d2-145">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="b49d2-146">*False* — учетные записи пользователей, переименованные в рамках этой операции, не отключаются.</span><span class="sxs-lookup"><span data-stu-id="b49d2-146">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="b49d2-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="b49d2-147">Response</span></span>

<span data-ttu-id="b49d2-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b49d2-148">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="b49d2-149">Пример</span><span class="sxs-lookup"><span data-stu-id="b49d2-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b49d2-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b49d2-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b49d2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b49d2-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b49d2-152">C#</span><span class="sxs-lookup"><span data-stu-id="b49d2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b49d2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b49d2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b49d2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b49d2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b49d2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b49d2-155">Response</span></span>

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
