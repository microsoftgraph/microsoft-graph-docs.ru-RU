---
title: Перечисление serviceConfigurationRecords
description: Получение списка объектов domainDnsRecord, которые требуются, чтобы включить службы для домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2880a8336d15b675cd5debc6008d8de8f4d191f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965540"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="faae3-103">Перечисление serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="faae3-103">List serviceConfigurationRecords</span></span>

> <span data-ttu-id="faae3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faae3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faae3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faae3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faae3-106">Получение списка объектов [domainDnsRecord](../resources/domaindnsrecord.md), которые требуются, чтобы включить службы для домена.</span><span class="sxs-lookup"><span data-stu-id="faae3-106">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="faae3-p102">Используйте возвращенный список для добавления записей в файле зоны домена. Это можно сделать с помощью регистратора доменных имен или путем настройки DNS-сервера.</span><span class="sxs-lookup"><span data-stu-id="faae3-p102">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="faae3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="faae3-109">Permissions</span></span>

<span data-ttu-id="faae3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faae3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="faae3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faae3-112">Permission type</span></span>      | <span data-ttu-id="faae3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="faae3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faae3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faae3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="faae3-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="faae3-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="faae3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faae3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faae3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faae3-117">Not supported.</span></span>    |
|<span data-ttu-id="faae3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faae3-118">Application</span></span> | <span data-ttu-id="faae3-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faae3-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="faae3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faae3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="faae3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="faae3-121">Optional query parameters</span></span>

<span data-ttu-id="faae3-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="faae3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="faae3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faae3-123">Request headers</span></span>

| <span data-ttu-id="faae3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="faae3-124">Name</span></span>      |<span data-ttu-id="faae3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="faae3-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="faae3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faae3-126">Authorization</span></span>  | <span data-ttu-id="faae3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faae3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="faae3-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faae3-129">Content-Type</span></span>  | <span data-ttu-id="faae3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="faae3-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="faae3-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="faae3-131">Request body</span></span>

<span data-ttu-id="faae3-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="faae3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faae3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="faae3-133">Response</span></span>

<span data-ttu-id="faae3-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domainDnsRecord](../resources/domaindnsrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="faae3-134">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faae3-135">Пример</span><span class="sxs-lookup"><span data-stu-id="faae3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="faae3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="faae3-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="faae3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="faae3-137">Response</span></span>
<span data-ttu-id="faae3-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faae3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
