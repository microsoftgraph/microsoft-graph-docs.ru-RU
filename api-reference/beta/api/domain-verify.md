---
title: 'domain: verify'
description: Проверка права собственности на домен.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56d6835f2df7c25e21393054cccfed0fc8570824
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433323"
---
# <a name="domain-verify"></a><span data-ttu-id="30c3e-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="30c3e-103">domain: verify</span></span>

<span data-ttu-id="30c3e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="30c3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30c3e-105">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="30c3e-105">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="30c3e-p101">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="30c3e-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="30c3e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30c3e-108">Permissions</span></span>

<span data-ttu-id="30c3e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30c3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="30c3e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30c3e-111">Permission type</span></span>      | <span data-ttu-id="30c3e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30c3e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30c3e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30c3e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="30c3e-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="30c3e-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="30c3e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30c3e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30c3e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30c3e-116">Not supported.</span></span>    |
|<span data-ttu-id="30c3e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30c3e-117">Application</span></span> | <span data-ttu-id="30c3e-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30c3e-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30c3e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30c3e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="30c3e-120">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="30c3e-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30c3e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30c3e-121">Request headers</span></span>

| <span data-ttu-id="30c3e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="30c3e-122">Name</span></span>       | <span data-ttu-id="30c3e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="30c3e-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="30c3e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30c3e-124">Authorization</span></span>  | <span data-ttu-id="30c3e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30c3e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="30c3e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30c3e-127">Content-Type</span></span>  | <span data-ttu-id="30c3e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30c3e-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="30c3e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30c3e-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="30c3e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="30c3e-130">Response</span></span>

<span data-ttu-id="30c3e-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="30c3e-131">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30c3e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="30c3e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30c3e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="30c3e-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="30c3e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="30c3e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```
# <a name="c"></a>[<span data-ttu-id="30c3e-135">C#</span><span class="sxs-lookup"><span data-stu-id="30c3e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30c3e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30c3e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30c3e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30c3e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="30c3e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="30c3e-138">Response</span></span>
<span data-ttu-id="30c3e-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30c3e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
