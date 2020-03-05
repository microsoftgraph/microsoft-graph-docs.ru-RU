---
title: Список serviceConfigurationRecords
description: Получает список объектов domainDnsRecord, необходимых для включения служб для домена.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 950a7d06d255367ae69481d8c0efb28c264992c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433568"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="e0fd6-103">Список serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="e0fd6-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="e0fd6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e0fd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0fd6-105">Получает список объектов [domainDnsRecord](../resources/domaindnsrecord.md) , необходимых для включения служб для домена.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="e0fd6-106">Используйте возвращенный список, чтобы добавить записи в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="e0fd6-107">Это можно сделать с помощью регистратора доменных имен или DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0fd6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0fd6-108">Permissions</span></span>

<span data-ttu-id="e0fd6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0fd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0fd6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0fd6-111">Permission type</span></span>      | <span data-ttu-id="e0fd6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0fd6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0fd6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0fd6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e0fd6-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0fd6-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="e0fd6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0fd6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0fd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-116">Not supported.</span></span>    |
|<span data-ttu-id="e0fd6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0fd6-117">Application</span></span> | <span data-ttu-id="e0fd6-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fd6-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0fd6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0fd6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0fd6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0fd6-120">Optional query parameters</span></span>

<span data-ttu-id="e0fd6-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0fd6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0fd6-122">Request headers</span></span>

| <span data-ttu-id="e0fd6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e0fd6-123">Name</span></span>      |<span data-ttu-id="e0fd6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e0fd6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0fd6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0fd6-125">Authorization</span></span>  | <span data-ttu-id="e0fd6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0fd6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0fd6-128">Content-Type</span></span>  | <span data-ttu-id="e0fd6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e0fd6-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0fd6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0fd6-130">Request body</span></span>

<span data-ttu-id="e0fd6-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0fd6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0fd6-132">Response</span></span>

<span data-ttu-id="e0fd6-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fd6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e0fd6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0fd6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0fd6-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e0fd6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0fd6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="e0fd6-137">C#</span><span class="sxs-lookup"><span data-stu-id="e0fd6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0fd6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0fd6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0fd6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0fd6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0fd6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0fd6-140">Response</span></span>
<span data-ttu-id="e0fd6-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0fd6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
