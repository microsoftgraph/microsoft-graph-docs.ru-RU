---
title: Проверка спискаDnsRecords
description: Извлечение списка объектов domainDnsRecord.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 52d3232824a56eb13dd625e1cbb081c5954bd032
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046421"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="ac1f6-103">Проверка спискаDnsRecords</span><span class="sxs-lookup"><span data-stu-id="ac1f6-103">List verificationDnsRecords</span></span>

<span data-ttu-id="ac1f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac1f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac1f6-105">Извлечение списка [объектов domainDnsRecord.](../resources/domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="ac1f6-105">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="ac1f6-106">Вы не можете использовать связанный домен с клиентом Azure AD до тех пор, пока не будет проверено право собственности.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-106">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="ac1f6-107">Чтобы проверить право собственности на домен, извлекайте записи проверки домена и добавьте сведения в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-107">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="ac1f6-108">Это можно сделать с помощью регистратора домена или конфигурации сервера DNS.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-108">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="ac1f6-109">Корневые домены требуют проверки.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-109">Root domains require verification.</span></span> <span data-ttu-id="ac1f6-110">Например, contoso.com требуется проверка.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-110">For example, contoso.com requires verification.</span></span> <span data-ttu-id="ac1f6-111">При проверке корневого домена автоматически проверяются поддомены корневого домена.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-111">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="ac1f6-112">Например, subdomain.contoso.com проверяется автоматически, если contoso.com проверено.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-112">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac1f6-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac1f6-113">Permissions</span></span>

<span data-ttu-id="ac1f6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac1f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ac1f6-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac1f6-116">Permission type</span></span>      | <span data-ttu-id="ac1f6-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac1f6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac1f6-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac1f6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="ac1f6-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac1f6-119">Directory.Read.All</span></span>    |
|<span data-ttu-id="ac1f6-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac1f6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac1f6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-121">Not supported.</span></span>    |
|<span data-ttu-id="ac1f6-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac1f6-122">Application</span></span> | <span data-ttu-id="ac1f6-123">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac1f6-123">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac1f6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac1f6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="ac1f6-125">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ac1f6-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ac1f6-126">Optional query parameters</span></span>

<span data-ttu-id="ac1f6-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac1f6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac1f6-128">Request headers</span></span>

| <span data-ttu-id="ac1f6-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ac1f6-129">Name</span></span>      |<span data-ttu-id="ac1f6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ac1f6-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac1f6-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac1f6-131">Authorization</span></span>  | <span data-ttu-id="ac1f6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac1f6-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac1f6-134">Content-Type</span></span>  | <span data-ttu-id="ac1f6-135">application/json</span><span class="sxs-lookup"><span data-stu-id="ac1f6-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac1f6-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac1f6-136">Request body</span></span>

<span data-ttu-id="ac1f6-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac1f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac1f6-138">Response</span></span>

<span data-ttu-id="ac1f6-139">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов domainDnsRecord](../resources/domaindnsrecord.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-139">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac1f6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ac1f6-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac1f6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac1f6-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ac1f6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac1f6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```
# <a name="c"></a>[<span data-ttu-id="ac1f6-143">C#</span><span class="sxs-lookup"><span data-stu-id="ac1f6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-verificationdnsrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac1f6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac1f6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-verificationdnsrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac1f6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac1f6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-verificationdnsrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac1f6-146">Java</span><span class="sxs-lookup"><span data-stu-id="ac1f6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-verificationdnsrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac1f6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac1f6-147">Response</span></span>

<span data-ttu-id="ac1f6-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac1f6-148">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
