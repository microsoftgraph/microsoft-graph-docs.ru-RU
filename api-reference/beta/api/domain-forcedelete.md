---
title: 'домен: Форцеделете'
description: Удаляет домен, используя асинхронную операцию.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1220513f2ba5abf2957fa8c0e550e22985d2635
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260482"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="2c80f-103">домен: Форцеделете</span><span class="sxs-lookup"><span data-stu-id="2c80f-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c80f-104">Удаляет домен, используя асинхронную операцию.</span><span class="sxs-lookup"><span data-stu-id="2c80f-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="2c80f-105">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="2c80f-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="2c80f-106">Переименовывает имя участника-пользователя, EmailAddress и ProxyAddress пользователей со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="2c80f-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="2c80f-107">Переименование EmailAddress групп со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="2c80f-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="2c80f-108">Переименовывает С identifieruris приложений со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="2c80f-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="2c80f-109">Если количество переименованных объектов больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="2c80f-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="2c80f-110">Если одно из переименованных приложений является приложением с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="2c80f-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="2c80f-111">После завершения удаления домена операции API для удаленного домена будут возвращать код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="2c80f-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="2c80f-112">Чтобы проверить удаление домена, можно выполнить [Получение домена](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="2c80f-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="2c80f-113">Если домен был успешно удален, в ответе будет возвращен код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="2c80f-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c80f-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c80f-114">Permissions</span></span>

<span data-ttu-id="2c80f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c80f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2c80f-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c80f-117">Permission type</span></span>      | <span data-ttu-id="2c80f-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c80f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c80f-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c80f-119">Delegated (work or school account)</span></span> | <span data-ttu-id="2c80f-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c80f-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c80f-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c80f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c80f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c80f-122">Not supported.</span></span>    |
|<span data-ttu-id="2c80f-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c80f-123">Application</span></span> | <span data-ttu-id="2c80f-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c80f-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c80f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c80f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="2c80f-126">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="2c80f-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c80f-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c80f-127">Request headers</span></span>

| <span data-ttu-id="2c80f-128">Имя</span><span class="sxs-lookup"><span data-stu-id="2c80f-128">Name</span></span>       | <span data-ttu-id="2c80f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2c80f-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c80f-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c80f-130">Authorization</span></span>  | <span data-ttu-id="2c80f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c80f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2c80f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c80f-133">Content-Type</span></span>  | <span data-ttu-id="2c80f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2c80f-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c80f-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c80f-135">Request body</span></span>

<span data-ttu-id="2c80f-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2c80f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c80f-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c80f-137">Parameter</span></span>    | <span data-ttu-id="2c80f-138">Тип</span><span class="sxs-lookup"><span data-stu-id="2c80f-138">Type</span></span>   |<span data-ttu-id="2c80f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2c80f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c80f-140">Дисаблеусераккаунтс</span><span class="sxs-lookup"><span data-stu-id="2c80f-140">disableUserAccounts</span></span>|<span data-ttu-id="2c80f-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c80f-141">Boolean</span></span>| <span data-ttu-id="2c80f-142">Возможность отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="2c80f-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="2c80f-143">Если учетная запись пользователя отключена, пользователь не может войти в систему.</span><span class="sxs-lookup"><span data-stu-id="2c80f-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="2c80f-144">*Значение true* (по умолчанию)-учетные записи пользователей, переименованные в рамках этой операции, отключены.</span><span class="sxs-lookup"><span data-stu-id="2c80f-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="2c80f-145">*False* — учетные записи пользователей, переименованные в рамках этой операции, не отключаются.</span><span class="sxs-lookup"><span data-stu-id="2c80f-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="2c80f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c80f-146">Response</span></span>

<span data-ttu-id="2c80f-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2c80f-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="2c80f-148">Пример</span><span class="sxs-lookup"><span data-stu-id="2c80f-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c80f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c80f-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="2c80f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c80f-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c80f-151">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2c80f-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c80f-152">C#</span><span class="sxs-lookup"><span data-stu-id="2c80f-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c80f-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c80f-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c80f-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2c80f-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
