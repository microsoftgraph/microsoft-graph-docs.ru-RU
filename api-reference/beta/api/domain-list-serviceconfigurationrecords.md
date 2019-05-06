---
title: Список serviceConfigurationRecords
description: Получает список объектов domainDnsRecord, необходимых для включения служб для домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3132b0d06415ec70e0252f8263baa95b47a2c253
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589235"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="75382-103">Список serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="75382-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="75382-104">Получает список объектов [domainDnsRecord](../resources/domaindnsrecord.md) , необходимых для включения служб для домена.</span><span class="sxs-lookup"><span data-stu-id="75382-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="75382-105">Используйте возвращенный список, чтобы добавить записи в файл зоны домена.</span><span class="sxs-lookup"><span data-stu-id="75382-105">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="75382-106">Это можно сделать с помощью регистратора доменных имен или DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="75382-106">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="75382-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75382-107">Permissions</span></span>

<span data-ttu-id="75382-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75382-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="75382-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75382-110">Permission type</span></span>      | <span data-ttu-id="75382-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75382-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75382-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75382-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75382-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="75382-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="75382-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75382-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75382-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75382-115">Not supported.</span></span>    |
|<span data-ttu-id="75382-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75382-116">Application</span></span> | <span data-ttu-id="75382-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75382-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75382-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75382-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75382-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75382-119">Optional query parameters</span></span>

<span data-ttu-id="75382-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75382-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75382-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75382-121">Request headers</span></span>

| <span data-ttu-id="75382-122">Имя</span><span class="sxs-lookup"><span data-stu-id="75382-122">Name</span></span>      |<span data-ttu-id="75382-123">Описание</span><span class="sxs-lookup"><span data-stu-id="75382-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75382-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75382-124">Authorization</span></span>  | <span data-ttu-id="75382-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75382-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75382-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75382-127">Content-Type</span></span>  | <span data-ttu-id="75382-128">application/json</span><span class="sxs-lookup"><span data-stu-id="75382-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="75382-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75382-129">Request body</span></span>

<span data-ttu-id="75382-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75382-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75382-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="75382-131">Response</span></span>

<span data-ttu-id="75382-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75382-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75382-133">Пример</span><span class="sxs-lookup"><span data-stu-id="75382-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75382-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="75382-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="75382-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="75382-135">Response</span></span>
<span data-ttu-id="75382-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75382-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="75382-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="75382-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="75382-139">Языках</span><span class="sxs-lookup"><span data-stu-id="75382-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceconfigurationrecords-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75382-140">Язык</span><span class="sxs-lookup"><span data-stu-id="75382-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceconfigurationrecords-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-serviceconfigurationrecords.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-serviceconfigurationrecords.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
