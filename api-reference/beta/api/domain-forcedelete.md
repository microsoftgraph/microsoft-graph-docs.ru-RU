---
title: 'домен: forceDelete'
description: Удаление домена, с помощью асинхронной операции.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527691"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="e423e-103">домен: forceDelete</span><span class="sxs-lookup"><span data-stu-id="e423e-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e423e-104">Удаление домена, с помощью асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="e423e-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="e423e-105">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e423e-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="e423e-106">Переименовывает имени участника-пользователя, EmailAddress и ProxyAddress пользователей с помощью ссылки на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="e423e-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="e423e-107">Переименовывает EmailAddress групп ссылок на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="e423e-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="e423e-108">Переименовывает identifierUris приложений с помощью ссылки на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="e423e-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="e423e-109">Если число объектов, чтобы переименовать больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="e423e-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="e423e-110">Если один из приложений, чтобы переименовать приложения нескольких развертываний, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="e423e-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="e423e-111">После завершения удаления домена операции API для удаленного домена возвращает код ответа HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="e423e-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="e423e-112">Чтобы подтвердить удаление домена, можно выполнить [Получение домена](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="e423e-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="e423e-113">Если домен был успешно удален, код ответа HTTP 404 будут возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="e423e-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="e423e-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e423e-114">Permissions</span></span>

<span data-ttu-id="e423e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e423e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e423e-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e423e-117">Permission type</span></span>      | <span data-ttu-id="e423e-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e423e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e423e-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e423e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="e423e-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e423e-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e423e-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e423e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e423e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e423e-122">Not supported.</span></span>    |
|<span data-ttu-id="e423e-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e423e-123">Application</span></span> | <span data-ttu-id="e423e-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e423e-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e423e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e423e-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="e423e-126">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e423e-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e423e-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e423e-127">Request headers</span></span>

| <span data-ttu-id="e423e-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e423e-128">Name</span></span>       | <span data-ttu-id="e423e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e423e-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e423e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e423e-130">Authorization</span></span>  | <span data-ttu-id="e423e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e423e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e423e-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e423e-133">Content-Type</span></span>  | <span data-ttu-id="e423e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e423e-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e423e-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e423e-135">Request body</span></span>

<span data-ttu-id="e423e-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e423e-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e423e-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="e423e-137">Parameter</span></span>    | <span data-ttu-id="e423e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e423e-138">Type</span></span>   |<span data-ttu-id="e423e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e423e-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e423e-140">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="e423e-140">disableUserAccounts</span></span>|<span data-ttu-id="e423e-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="e423e-141">Boolean</span></span>| <span data-ttu-id="e423e-142">Параметр, чтобы отключить переименованной учетных записей.</span><span class="sxs-lookup"><span data-stu-id="e423e-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="e423e-143">Если учетная запись пользователя отключена, пользователь не разрешено вход.</span><span class="sxs-lookup"><span data-stu-id="e423e-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="e423e-144">*Значение true* (по умолчанию) — переименовано в рамках этой операции учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="e423e-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="e423e-145">*False* — переименовано в рамках этой операции учетные записи пользователей не отключены.</span><span class="sxs-lookup"><span data-stu-id="e423e-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="e423e-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="e423e-146">Response</span></span>

<span data-ttu-id="e423e-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e423e-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="e423e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e423e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e423e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e423e-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="e423e-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="e423e-150">Response</span></span>

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
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
