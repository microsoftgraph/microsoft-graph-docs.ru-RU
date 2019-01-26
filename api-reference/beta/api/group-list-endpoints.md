---
title: Перечисление конечных точек
description: Получение списка объектов конечной точки.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4f6d5d1fc8578f390dce0fece668a851c47032a7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575858"
---
# <a name="list-endpoints"></a><span data-ttu-id="b5da6-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="b5da6-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5da6-104">Получение списка объектов [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="b5da6-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5da6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5da6-105">Permissions</span></span>
<span data-ttu-id="b5da6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5da6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5da6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5da6-108">Permission type</span></span>      | <span data-ttu-id="b5da6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5da6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5da6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5da6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5da6-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5da6-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5da6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5da6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5da6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5da6-113">Not supported.</span></span>    |
|<span data-ttu-id="b5da6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5da6-114">Application</span></span> | <span data-ttu-id="b5da6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5da6-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5da6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5da6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5da6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5da6-117">Optional query parameters</span></span>
<span data-ttu-id="b5da6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5da6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5da6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5da6-119">Request headers</span></span>
| <span data-ttu-id="b5da6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b5da6-120">Name</span></span>      |<span data-ttu-id="b5da6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b5da6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5da6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5da6-122">Authorization</span></span>  | <span data-ttu-id="b5da6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5da6-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b5da6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5da6-125">Content-Type</span></span>   | <span data-ttu-id="b5da6-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="b5da6-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5da6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5da6-127">Request body</span></span>
<span data-ttu-id="b5da6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5da6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5da6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5da6-129">Response</span></span>

<span data-ttu-id="b5da6-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [конечной точки](../resources/endpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b5da6-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5da6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b5da6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5da6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5da6-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="b5da6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5da6-133">Response</span></span>
<span data-ttu-id="b5da6-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5da6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
