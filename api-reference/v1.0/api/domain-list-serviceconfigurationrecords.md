---
title: Список serviceConfigurationRecords
description: Получает список объектов domainDnsRecord, необходимых для включения служб для домена.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1511264ab304ae317686ea99fd8dbe8014f11132
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517876"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="8c72a-103">Список serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="8c72a-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="8c72a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c72a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c72a-105">Получает список объектов [domainDnsRecord](../resources/domaindnsrecord.md) , необходимых для включения служб для домена.</span><span class="sxs-lookup"><span data-stu-id="8c72a-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="8c72a-106">Используйте возвращенный список, чтобы добавить записи в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="8c72a-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="8c72a-107">Это можно сделать с помощью регистратора доменных имен или DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="8c72a-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c72a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c72a-108">Permissions</span></span>

<span data-ttu-id="8c72a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c72a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c72a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c72a-111">Permission type</span></span>      | <span data-ttu-id="8c72a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c72a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c72a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c72a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c72a-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c72a-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="8c72a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c72a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c72a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c72a-116">Not supported.</span></span>    |
|<span data-ttu-id="8c72a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c72a-117">Application</span></span> | <span data-ttu-id="8c72a-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c72a-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c72a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c72a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c72a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c72a-120">Optional query parameters</span></span>

<span data-ttu-id="8c72a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8c72a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c72a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c72a-122">Request headers</span></span>

| <span data-ttu-id="8c72a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8c72a-123">Name</span></span>      |<span data-ttu-id="8c72a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8c72a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c72a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c72a-125">Authorization</span></span>  | <span data-ttu-id="8c72a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c72a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c72a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c72a-128">Content-Type</span></span>  | <span data-ttu-id="8c72a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8c72a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c72a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c72a-130">Request body</span></span>

<span data-ttu-id="8c72a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c72a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c72a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c72a-132">Response</span></span>

<span data-ttu-id="8c72a-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c72a-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c72a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8c72a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c72a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c72a-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c72a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c72a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="8c72a-137">C#</span><span class="sxs-lookup"><span data-stu-id="8c72a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c72a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c72a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c72a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c72a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c72a-140">Java</span><span class="sxs-lookup"><span data-stu-id="8c72a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c72a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c72a-141">Response</span></span>
<span data-ttu-id="8c72a-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c72a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
