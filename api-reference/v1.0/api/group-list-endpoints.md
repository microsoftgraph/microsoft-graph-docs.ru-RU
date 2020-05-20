---
title: Перечисление конечных точек
description: Получение списка объектов конечной точки.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 738ccf502398a419dc54c12824cf6ce53654372e
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290415"
---
# <a name="list-endpoints"></a><span data-ttu-id="d78b0-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="d78b0-103">List endpoints</span></span>

<span data-ttu-id="d78b0-104">Получение списка объектов [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="d78b0-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d78b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d78b0-105">Permissions</span></span>
<span data-ttu-id="d78b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d78b0-108">Permission type</span></span>      | <span data-ttu-id="d78b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d78b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d78b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d78b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d78b0-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78b0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d78b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d78b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d78b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78b0-113">Not supported.</span></span>    |
|<span data-ttu-id="d78b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d78b0-114">Application</span></span> | <span data-ttu-id="d78b0-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78b0-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d78b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d78b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d78b0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d78b0-117">Optional query parameters</span></span>
<span data-ttu-id="d78b0-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d78b0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d78b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d78b0-119">Request headers</span></span>
| <span data-ttu-id="d78b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d78b0-120">Name</span></span>      |<span data-ttu-id="d78b0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d78b0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d78b0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d78b0-122">Authorization</span></span>  | <span data-ttu-id="d78b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d78b0-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d78b0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d78b0-125">Content-Type</span></span>   | <span data-ttu-id="d78b0-126">Приложение/JSON</span><span class="sxs-lookup"><span data-stu-id="d78b0-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d78b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d78b0-127">Request body</span></span>
<span data-ttu-id="d78b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d78b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d78b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78b0-129">Response</span></span>

<span data-ttu-id="d78b0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Endpoint](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d78b0-130">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d78b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d78b0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d78b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d78b0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d78b0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d78b0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```

### <a name="response"></a><span data-ttu-id="d78b0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78b0-134">Response</span></span>
<span data-ttu-id="d78b0-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d78b0-135">Here is an example of the response.</span></span>
><span data-ttu-id="d78b0-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d78b0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
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
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
