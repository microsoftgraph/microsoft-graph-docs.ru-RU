---
title: Перечисление verificationDnsRecords
description: Получение списка объектов domainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 9f9fd611b590c3ace61394309637340288cf7bb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353104"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="70b17-103">Перечисление verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="70b17-103">List verificationDnsRecords</span></span>

<span data-ttu-id="70b17-104">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="70b17-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="70b17-p101">Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Чтобы подтвердить владение доменом, получите записи проверки домена и добавьте сведения в файл зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="70b17-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="70b17-p102">Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.</span><span class="sxs-lookup"><span data-stu-id="70b17-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="70b17-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70b17-112">Permissions</span></span>

<span data-ttu-id="70b17-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70b17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70b17-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70b17-115">Permission type</span></span>      | <span data-ttu-id="70b17-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70b17-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70b17-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70b17-117">Delegated (work or school account)</span></span> | <span data-ttu-id="70b17-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="70b17-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="70b17-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70b17-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70b17-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70b17-120">Not supported.</span></span>    |
|<span data-ttu-id="70b17-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70b17-121">Application</span></span> | <span data-ttu-id="70b17-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b17-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70b17-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70b17-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="70b17-124">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="70b17-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="70b17-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70b17-125">Optional query parameters</span></span>

<span data-ttu-id="70b17-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70b17-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70b17-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70b17-127">Request headers</span></span>

| <span data-ttu-id="70b17-128">Имя</span><span class="sxs-lookup"><span data-stu-id="70b17-128">Name</span></span>      |<span data-ttu-id="70b17-129">Описание</span><span class="sxs-lookup"><span data-stu-id="70b17-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70b17-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70b17-130">Authorization</span></span>  | <span data-ttu-id="70b17-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70b17-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70b17-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70b17-133">Content-Type</span></span>  | <span data-ttu-id="70b17-134">application/json</span><span class="sxs-lookup"><span data-stu-id="70b17-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70b17-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70b17-135">Request body</span></span>

<span data-ttu-id="70b17-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70b17-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70b17-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="70b17-137">Response</span></span>

<span data-ttu-id="70b17-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70b17-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70b17-139">Пример</span><span class="sxs-lookup"><span data-stu-id="70b17-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70b17-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="70b17-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="70b17-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="70b17-141">Response</span></span>

<span data-ttu-id="70b17-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70b17-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->