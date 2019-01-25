---
title: Перечисление verificationDnsRecords
description: Получение списка объектов domainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a470f6bddb9cade8083afb3eb5d5cf76cf4dba32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522842"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="66f06-103">Перечисление verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="66f06-103">List verificationDnsRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f06-104">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="66f06-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="66f06-p101">Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Чтобы подтвердить владение доменом, получите записи проверки домена и добавьте сведения в файл зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="66f06-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="66f06-p102">Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.</span><span class="sxs-lookup"><span data-stu-id="66f06-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="66f06-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66f06-112">Permissions</span></span>

<span data-ttu-id="66f06-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66f06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66f06-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66f06-115">Permission type</span></span>      | <span data-ttu-id="66f06-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66f06-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66f06-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66f06-117">Delegated (work or school account)</span></span> | <span data-ttu-id="66f06-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="66f06-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="66f06-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66f06-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66f06-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66f06-120">Not supported.</span></span>    |
|<span data-ttu-id="66f06-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66f06-121">Application</span></span> | <span data-ttu-id="66f06-122">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66f06-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66f06-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66f06-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="66f06-124">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="66f06-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="66f06-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66f06-125">Optional query parameters</span></span>

<span data-ttu-id="66f06-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66f06-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66f06-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66f06-127">Request headers</span></span>

| <span data-ttu-id="66f06-128">Имя</span><span class="sxs-lookup"><span data-stu-id="66f06-128">Name</span></span>      |<span data-ttu-id="66f06-129">Описание</span><span class="sxs-lookup"><span data-stu-id="66f06-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66f06-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66f06-130">Authorization</span></span>  | <span data-ttu-id="66f06-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66f06-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66f06-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66f06-133">Content-Type</span></span>  | <span data-ttu-id="66f06-134">application/json</span><span class="sxs-lookup"><span data-stu-id="66f06-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="66f06-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66f06-135">Request body</span></span>

<span data-ttu-id="66f06-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66f06-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66f06-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="66f06-137">Response</span></span>

<span data-ttu-id="66f06-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66f06-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66f06-139">Пример</span><span class="sxs-lookup"><span data-stu-id="66f06-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66f06-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="66f06-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="66f06-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="66f06-141">Response</span></span>

<span data-ttu-id="66f06-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66f06-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
