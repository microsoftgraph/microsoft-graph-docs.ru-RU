---
title: 'domain: verify'
description: Проверка права собственности на домен.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ade9192e3926b6030b564f05ea5de653a45e66e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417005"
---
# <a name="domain-verify"></a><span data-ttu-id="4082d-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="4082d-103">domain: verify</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4082d-104">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="4082d-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="4082d-p101">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="4082d-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="4082d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4082d-107">Permissions</span></span>

<span data-ttu-id="4082d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4082d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4082d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4082d-110">Permission type</span></span>      | <span data-ttu-id="4082d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4082d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4082d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4082d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4082d-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4082d-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="4082d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4082d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4082d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4082d-115">Not supported.</span></span>    |
|<span data-ttu-id="4082d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4082d-116">Application</span></span> | <span data-ttu-id="4082d-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4082d-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4082d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4082d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="4082d-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="4082d-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4082d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4082d-120">Request headers</span></span>

| <span data-ttu-id="4082d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4082d-121">Name</span></span>       | <span data-ttu-id="4082d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4082d-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4082d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4082d-123">Authorization</span></span>  | <span data-ttu-id="4082d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4082d-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4082d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4082d-126">Content-Type</span></span>  | <span data-ttu-id="4082d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4082d-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4082d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4082d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4082d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4082d-129">Response</span></span>

<span data-ttu-id="4082d-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4082d-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4082d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4082d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4082d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4082d-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4082d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4082d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4082d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4082d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4082d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4082d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4082d-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4082d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4082d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4082d-137">Response</span></span>
<span data-ttu-id="4082d-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4082d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
