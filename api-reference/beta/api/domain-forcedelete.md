---
title: 'домен: forceDelete'
description: Удаление домена, с помощью асинхронной операции.
ms.openlocfilehash: 590ba49a4aff99385a2584b3d544d7682a030eb6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076239"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="67076-103">домен: forceDelete</span><span class="sxs-lookup"><span data-stu-id="67076-103">domain: forceDelete</span></span>

> <span data-ttu-id="67076-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67076-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67076-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67076-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67076-106">Удаление домена, с помощью асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="67076-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="67076-107">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="67076-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="67076-108">Переименовывает имени участника-пользователя, EmailAddress и ProxyAddress пользователей с помощью ссылки на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="67076-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="67076-109">Переименовывает EmailAddress групп ссылок на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="67076-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="67076-110">Переименовывает identifierUris приложений с помощью ссылки на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="67076-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="67076-111">Если число объектов, чтобы переименовать больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="67076-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="67076-112">Если один из приложений, чтобы переименовать приложения нескольких развертываний, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="67076-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="67076-113">После завершения удаления домена операции API для удаленного домена возвращает код ответа HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="67076-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="67076-114">Чтобы подтвердить удаление домена, можно выполнить [Получение домена](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="67076-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="67076-115">Если домен был успешно удален, код ответа HTTP 404 будут возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="67076-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="67076-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67076-116">Permissions</span></span>

<span data-ttu-id="67076-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67076-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67076-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67076-119">Permission type</span></span>      | <span data-ttu-id="67076-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67076-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67076-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67076-121">Delegated (work or school account)</span></span> | <span data-ttu-id="67076-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67076-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67076-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67076-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67076-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67076-124">Not supported.</span></span>    |
|<span data-ttu-id="67076-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67076-125">Application</span></span> | <span data-ttu-id="67076-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67076-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67076-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67076-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="67076-128">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="67076-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67076-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67076-129">Request headers</span></span>

| <span data-ttu-id="67076-130">Имя</span><span class="sxs-lookup"><span data-stu-id="67076-130">Name</span></span>       | <span data-ttu-id="67076-131">Описание</span><span class="sxs-lookup"><span data-stu-id="67076-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67076-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67076-132">Authorization</span></span>  | <span data-ttu-id="67076-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67076-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="67076-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67076-135">Content-Type</span></span>  | <span data-ttu-id="67076-136">application/json</span><span class="sxs-lookup"><span data-stu-id="67076-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="67076-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67076-137">Request body</span></span>

<span data-ttu-id="67076-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="67076-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67076-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="67076-139">Parameter</span></span>    | <span data-ttu-id="67076-140">Тип</span><span class="sxs-lookup"><span data-stu-id="67076-140">Type</span></span>   |<span data-ttu-id="67076-141">Description</span><span class="sxs-lookup"><span data-stu-id="67076-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67076-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="67076-142">disableUserAccounts</span></span>|<span data-ttu-id="67076-143">Логический</span><span class="sxs-lookup"><span data-stu-id="67076-143">Boolean</span></span>| <span data-ttu-id="67076-144">Параметр, чтобы отключить переименованной учетных записей.</span><span class="sxs-lookup"><span data-stu-id="67076-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="67076-145">Если учетная запись пользователя отключена, пользователь не разрешено вход.</span><span class="sxs-lookup"><span data-stu-id="67076-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="67076-146">*Значение true* (по умолчанию) — переименовано в рамках этой операции учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="67076-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="67076-147">*False* — переименовано в рамках этой операции учетные записи пользователей не отключены.</span><span class="sxs-lookup"><span data-stu-id="67076-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="67076-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="67076-148">Response</span></span>

<span data-ttu-id="67076-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="67076-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="67076-150">Пример</span><span class="sxs-lookup"><span data-stu-id="67076-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67076-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="67076-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="67076-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="67076-152">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->