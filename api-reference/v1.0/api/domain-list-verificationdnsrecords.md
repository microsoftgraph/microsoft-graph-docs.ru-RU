---
title: Список verificationDnsRecords
description: Получение списка объектов domainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecb3969370af6782bc8f8c7302fed07919ed15ba
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461234"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="a1fc5-103">Список verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="a1fc5-103">List verificationDnsRecords</span></span>

<span data-ttu-id="a1fc5-104">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="a1fc5-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="a1fc5-105">Вы не можете использовать связанный домен с клиентом Azure AD, пока не будет проверено владение.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-105">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="a1fc5-106">Чтобы проверить владение доменом, извлеките записи проверки домена и добавьте сведения в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-106">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="a1fc5-107">Это можно сделать с помощью регистратора доменных имен или DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-107">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="a1fc5-108">Корневые домены требуют проверки.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-108">Root domains require verification.</span></span> <span data-ttu-id="a1fc5-109">Например, для contoso.com требуется проверка.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-109">For example, contoso.com requires verification.</span></span> <span data-ttu-id="a1fc5-110">При проверке корневого домена автоматически проверяются дочерние домены корневого домена.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-110">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="a1fc5-111">Например, subdomain.contoso.com автоматически проверяется, если contoso.com проверено.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-111">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1fc5-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1fc5-112">Permissions</span></span>

<span data-ttu-id="a1fc5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1fc5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a1fc5-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1fc5-115">Permission type</span></span>      | <span data-ttu-id="a1fc5-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1fc5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1fc5-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1fc5-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a1fc5-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1fc5-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="a1fc5-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1fc5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1fc5-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-120">Not supported.</span></span>    |
|<span data-ttu-id="a1fc5-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1fc5-121">Application</span></span> | <span data-ttu-id="a1fc5-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1fc5-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1fc5-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1fc5-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="a1fc5-124">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a1fc5-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1fc5-125">Optional query parameters</span></span>

<span data-ttu-id="a1fc5-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1fc5-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1fc5-127">Request headers</span></span>

| <span data-ttu-id="a1fc5-128">Имя</span><span class="sxs-lookup"><span data-stu-id="a1fc5-128">Name</span></span>      |<span data-ttu-id="a1fc5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a1fc5-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1fc5-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1fc5-130">Authorization</span></span>  | <span data-ttu-id="a1fc5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1fc5-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1fc5-133">Content-Type</span></span>  | <span data-ttu-id="a1fc5-134">application/json</span><span class="sxs-lookup"><span data-stu-id="a1fc5-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1fc5-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1fc5-135">Request body</span></span>

<span data-ttu-id="a1fc5-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1fc5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1fc5-137">Response</span></span>

<span data-ttu-id="a1fc5-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1fc5-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a1fc5-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1fc5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1fc5-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a1fc5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1fc5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1fc5-142">C#</span><span class="sxs-lookup"><span data-stu-id="a1fc5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-verificationdnsrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1fc5-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1fc5-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-verificationdnsrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1fc5-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a1fc5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-verificationdnsrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a1fc5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1fc5-145">Response</span></span>

<span data-ttu-id="a1fc5-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1fc5-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
