---
title: 'домен: Форцеделете'
description: Удаляет домен, используя асинхронную операцию.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454934"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="7b328-103">домен: Форцеделете</span><span class="sxs-lookup"><span data-stu-id="7b328-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b328-104">Удаляет домен, используя асинхронную операцию.</span><span class="sxs-lookup"><span data-stu-id="7b328-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="7b328-105">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7b328-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="7b328-106">Переименовывает имя участника-пользователя, EmailAddress и ProxyAddress пользователей со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="7b328-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="7b328-107">Переименование EmailAddress групп со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="7b328-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="7b328-108">Переименовывает С identifieruris приложений со ссылками на удаленный домен.</span><span class="sxs-lookup"><span data-stu-id="7b328-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="7b328-109">Если количество переименованных объектов больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="7b328-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="7b328-110">Если одно из переименованных приложений является приложением с несколькими клиентами, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="7b328-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="7b328-111">После завершения удаления домена операции API для удаленного домена будут возвращать код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="7b328-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="7b328-112">Чтобы проверить удаление домена, можно выполнить [Получение домена](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="7b328-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="7b328-113">Если домен был успешно удален, в ответе будет возвращен код HTTP-ответа 404.</span><span class="sxs-lookup"><span data-stu-id="7b328-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b328-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b328-114">Permissions</span></span>

<span data-ttu-id="7b328-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b328-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7b328-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b328-117">Permission type</span></span>      | <span data-ttu-id="7b328-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b328-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b328-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b328-119">Delegated (work or school account)</span></span> | <span data-ttu-id="7b328-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b328-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b328-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b328-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b328-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b328-122">Not supported.</span></span>    |
|<span data-ttu-id="7b328-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b328-123">Application</span></span> | <span data-ttu-id="7b328-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b328-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b328-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b328-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="7b328-126">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="7b328-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b328-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b328-127">Request headers</span></span>

| <span data-ttu-id="7b328-128">Имя</span><span class="sxs-lookup"><span data-stu-id="7b328-128">Name</span></span>       | <span data-ttu-id="7b328-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7b328-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b328-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b328-130">Authorization</span></span>  | <span data-ttu-id="7b328-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b328-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="7b328-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b328-133">Content-Type</span></span>  | <span data-ttu-id="7b328-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7b328-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b328-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b328-135">Request body</span></span>

<span data-ttu-id="7b328-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7b328-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b328-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b328-137">Parameter</span></span>    | <span data-ttu-id="7b328-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7b328-138">Type</span></span>   |<span data-ttu-id="7b328-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7b328-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b328-140">Дисаблеусераккаунтс</span><span class="sxs-lookup"><span data-stu-id="7b328-140">disableUserAccounts</span></span>|<span data-ttu-id="7b328-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b328-141">Boolean</span></span>| <span data-ttu-id="7b328-142">Возможность отключения переименованных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b328-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="7b328-143">Если учетная запись пользователя отключена, пользователь не может войти в систему.</span><span class="sxs-lookup"><span data-stu-id="7b328-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="7b328-144">*Значение true* (по умолчанию)-учетные записи пользователей, переименованные в рамках этой операции, отключены.</span><span class="sxs-lookup"><span data-stu-id="7b328-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="7b328-145">*False* — учетные записи пользователей, переименованные в рамках этой операции, не отключаются.</span><span class="sxs-lookup"><span data-stu-id="7b328-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="7b328-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b328-146">Response</span></span>

<span data-ttu-id="7b328-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7b328-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="7b328-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7b328-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b328-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b328-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="7b328-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b328-150">Response</span></span>

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
