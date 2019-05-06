---
title: 'domain: verify'
description: Проверка права собственности на домен.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2d3139a9911be2f6e813f7e40051bd2286f0349e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589463"
---
# <a name="domain-verify"></a><span data-ttu-id="5a603-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="5a603-103">domain: verify</span></span>

<span data-ttu-id="5a603-104">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="5a603-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="5a603-p101">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="5a603-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a603-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a603-107">Permissions</span></span>

<span data-ttu-id="5a603-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a603-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a603-110">Permission type</span></span>      | <span data-ttu-id="5a603-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a603-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a603-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a603-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a603-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a603-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="5a603-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a603-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a603-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a603-115">Not supported.</span></span>    |
|<span data-ttu-id="5a603-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a603-116">Application</span></span> | <span data-ttu-id="5a603-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a603-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a603-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a603-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="5a603-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="5a603-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a603-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a603-120">Request headers</span></span>

| <span data-ttu-id="5a603-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5a603-121">Name</span></span>       | <span data-ttu-id="5a603-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a603-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5a603-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a603-123">Authorization</span></span>  | <span data-ttu-id="5a603-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a603-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5a603-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a603-126">Content-Type</span></span>  | <span data-ttu-id="5a603-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5a603-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a603-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a603-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5a603-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a603-129">Response</span></span>

<span data-ttu-id="5a603-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a603-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a603-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5a603-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a603-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a603-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="5a603-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a603-133">Response</span></span>
<span data-ttu-id="5a603-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a603-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a603-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5a603-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a603-137">Языках</span><span class="sxs-lookup"><span data-stu-id="5a603-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_verify-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a603-138">Язык</span><span class="sxs-lookup"><span data-stu-id="5a603-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_verify-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
