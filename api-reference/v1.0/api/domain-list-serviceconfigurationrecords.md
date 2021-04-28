---
title: Служба ListConfigurationRecords
description: Извлекает список объектов domainDnsRecord, необходимых для обеспечения служб для домена.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cb04790296aa1c6e1c934c8d37db28e9d1cd7620
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054065"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="d5e91-103">Служба ListConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="d5e91-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="d5e91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5e91-105">Извлекает список [объектов domainDnsRecord,](../resources/domaindnsrecord.md) необходимых для обеспечения служб для домена.</span><span class="sxs-lookup"><span data-stu-id="d5e91-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="d5e91-106">Используйте возвращенный список, чтобы добавить записи в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="d5e91-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="d5e91-107">Это можно сделать с помощью регистратора домена или конфигурации сервера DNS.</span><span class="sxs-lookup"><span data-stu-id="d5e91-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e91-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5e91-108">Permissions</span></span>

<span data-ttu-id="d5e91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5e91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5e91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5e91-111">Permission type</span></span>      | <span data-ttu-id="d5e91-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5e91-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5e91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5e91-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d5e91-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5e91-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="d5e91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5e91-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5e91-116">Not supported.</span></span>    |
|<span data-ttu-id="d5e91-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5e91-117">Application</span></span> | <span data-ttu-id="d5e91-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5e91-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5e91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5e91-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5e91-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5e91-120">Optional query parameters</span></span>

<span data-ttu-id="d5e91-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d5e91-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5e91-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5e91-122">Request headers</span></span>

| <span data-ttu-id="d5e91-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d5e91-123">Name</span></span>      |<span data-ttu-id="d5e91-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e91-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5e91-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5e91-125">Authorization</span></span>  | <span data-ttu-id="d5e91-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5e91-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5e91-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5e91-128">Content-Type</span></span>  | <span data-ttu-id="d5e91-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d5e91-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5e91-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5e91-130">Request body</span></span>

<span data-ttu-id="d5e91-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5e91-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5e91-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5e91-132">Response</span></span>

<span data-ttu-id="d5e91-133">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов domainDnsRecord](../resources/domaindnsrecord.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d5e91-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5e91-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d5e91-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5e91-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5e91-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5e91-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e91-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="d5e91-137">C#</span><span class="sxs-lookup"><span data-stu-id="d5e91-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5e91-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e91-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5e91-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5e91-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5e91-140">Java</span><span class="sxs-lookup"><span data-stu-id="d5e91-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d5e91-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5e91-141">Response</span></span>
<span data-ttu-id="d5e91-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5e91-142">Note: The response object shown here might be shortened for readability.</span></span>
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
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
