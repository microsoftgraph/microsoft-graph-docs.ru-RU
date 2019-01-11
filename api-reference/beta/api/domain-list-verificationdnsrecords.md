---
title: Перечисление verificationDnsRecords
description: Получение списка объектов domainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 335fd90dc56903061f1c5c5bb86672de1a438fcb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874902"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="d1ae1-103">Перечисление verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="d1ae1-103">List verificationDnsRecords</span></span>

> <span data-ttu-id="d1ae1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1ae1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1ae1-106">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="d1ae1-106">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="d1ae1-p102">Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Чтобы подтвердить владение доменом, получите записи проверки домена и добавьте сведения в файл зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-p102">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="d1ae1-p103">Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-p103">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1ae1-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ae1-114">Permissions</span></span>

<span data-ttu-id="d1ae1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1ae1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d1ae1-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ae1-117">Permission type</span></span>      | <span data-ttu-id="d1ae1-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1ae1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1ae1-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1ae1-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d1ae1-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1ae1-120">Directory.Read.All</span></span>    |
|<span data-ttu-id="d1ae1-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1ae1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1ae1-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-122">Not supported.</span></span>    |
|<span data-ttu-id="d1ae1-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1ae1-123">Application</span></span> | <span data-ttu-id="d1ae1-124">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ae1-124">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1ae1-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1ae1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="d1ae1-126">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d1ae1-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1ae1-127">Optional query parameters</span></span>

<span data-ttu-id="d1ae1-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ae1-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1ae1-129">Request headers</span></span>

| <span data-ttu-id="d1ae1-130">Имя</span><span class="sxs-lookup"><span data-stu-id="d1ae1-130">Name</span></span>      |<span data-ttu-id="d1ae1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1ae1-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1ae1-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1ae1-132">Authorization</span></span>  | <span data-ttu-id="d1ae1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1ae1-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1ae1-135">Content-Type</span></span>  | <span data-ttu-id="d1ae1-136">application/json</span><span class="sxs-lookup"><span data-stu-id="d1ae1-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1ae1-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1ae1-137">Request body</span></span>

<span data-ttu-id="d1ae1-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1ae1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ae1-139">Response</span></span>

<span data-ttu-id="d1ae1-140">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-140">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ae1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d1ae1-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1ae1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1ae1-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="d1ae1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ae1-143">Response</span></span>

<span data-ttu-id="d1ae1-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1ae1-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
