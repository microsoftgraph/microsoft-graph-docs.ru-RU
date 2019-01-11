---
title: Перечисление serviceConfigurationRecords
description: Получение списка объектов domainDnsRecord, которые требуются, чтобы включить службы для домена.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 958115620d9cf1e8a108c08004bfb124328f15b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825335"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="ce9ef-103">Перечисление serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="ce9ef-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="ce9ef-104">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md), которые требуются, чтобы включить службы для домена.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="ce9ef-p101">Используйте возвращенный список для добавления записей в файле зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce9ef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce9ef-107">Permissions</span></span>

<span data-ttu-id="ce9ef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce9ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ce9ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce9ef-110">Permission type</span></span>      | <span data-ttu-id="ce9ef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce9ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce9ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce9ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce9ef-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce9ef-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="ce9ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce9ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce9ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-115">Not supported.</span></span>    |
|<span data-ttu-id="ce9ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce9ef-116">Application</span></span> | <span data-ttu-id="ce9ef-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce9ef-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce9ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce9ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce9ef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce9ef-119">Optional query parameters</span></span>

<span data-ttu-id="ce9ef-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce9ef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce9ef-121">Request headers</span></span>

| <span data-ttu-id="ce9ef-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ce9ef-122">Name</span></span>      |<span data-ttu-id="ce9ef-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ce9ef-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce9ef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce9ef-124">Authorization</span></span>  | <span data-ttu-id="ce9ef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce9ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce9ef-127">Content-Type</span></span>  | <span data-ttu-id="ce9ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ce9ef-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce9ef-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce9ef-129">Request body</span></span>

<span data-ttu-id="ce9ef-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce9ef-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9ef-131">Response</span></span>

<span data-ttu-id="ce9ef-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce9ef-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ce9ef-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce9ef-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce9ef-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="ce9ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9ef-135">Response</span></span>
<span data-ttu-id="ce9ef-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce9ef-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
