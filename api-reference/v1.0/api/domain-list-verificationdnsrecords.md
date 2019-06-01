---
title: Список verificationDnsRecords
description: Получение списка объектов domainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91cfde034ce2633d7673fa88468504c11ed1e48a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655644"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="27f24-103">Список verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="27f24-103">List verificationDnsRecords</span></span>

<span data-ttu-id="27f24-104">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="27f24-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="27f24-105">Вы не можете использовать связанный домен с клиентом Azure AD, пока не будет проверено владение.</span><span class="sxs-lookup"><span data-stu-id="27f24-105">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="27f24-106">Чтобы проверить владение доменом, извлеките записи проверки домена и добавьте сведения в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="27f24-106">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="27f24-107">Это можно сделать с помощью регистратора доменных имен или DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="27f24-107">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="27f24-108">Корневые домены требуют проверки.</span><span class="sxs-lookup"><span data-stu-id="27f24-108">Root domains require verification.</span></span> <span data-ttu-id="27f24-109">Например, для contoso.com требуется проверка.</span><span class="sxs-lookup"><span data-stu-id="27f24-109">For example, contoso.com requires verification.</span></span> <span data-ttu-id="27f24-110">При проверке корневого домена автоматически проверяются дочерние домены корневого домена.</span><span class="sxs-lookup"><span data-stu-id="27f24-110">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="27f24-111">Например, subdomain.contoso.com автоматически проверяется, если contoso.com проверено.</span><span class="sxs-lookup"><span data-stu-id="27f24-111">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="27f24-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27f24-112">Permissions</span></span>

<span data-ttu-id="27f24-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27f24-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27f24-115">Permission type</span></span>      | <span data-ttu-id="27f24-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27f24-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27f24-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27f24-117">Delegated (work or school account)</span></span> | <span data-ttu-id="27f24-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="27f24-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="27f24-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27f24-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27f24-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f24-120">Not supported.</span></span>    |
|<span data-ttu-id="27f24-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27f24-121">Application</span></span> | <span data-ttu-id="27f24-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f24-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27f24-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27f24-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="27f24-124">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="27f24-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="27f24-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27f24-125">Optional query parameters</span></span>

<span data-ttu-id="27f24-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="27f24-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27f24-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27f24-127">Request headers</span></span>

| <span data-ttu-id="27f24-128">Имя</span><span class="sxs-lookup"><span data-stu-id="27f24-128">Name</span></span>      |<span data-ttu-id="27f24-129">Описание</span><span class="sxs-lookup"><span data-stu-id="27f24-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27f24-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27f24-130">Authorization</span></span>  | <span data-ttu-id="27f24-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27f24-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27f24-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27f24-133">Content-Type</span></span>  | <span data-ttu-id="27f24-134">application/json</span><span class="sxs-lookup"><span data-stu-id="27f24-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="27f24-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27f24-135">Request body</span></span>

<span data-ttu-id="27f24-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27f24-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27f24-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="27f24-137">Response</span></span>

<span data-ttu-id="27f24-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27f24-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27f24-139">Пример</span><span class="sxs-lookup"><span data-stu-id="27f24-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27f24-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="27f24-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="27f24-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="27f24-141">Response</span></span>

<span data-ttu-id="27f24-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27f24-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27f24-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="27f24-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27f24-145">C#</span><span class="sxs-lookup"><span data-stu-id="27f24-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27f24-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="27f24-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
