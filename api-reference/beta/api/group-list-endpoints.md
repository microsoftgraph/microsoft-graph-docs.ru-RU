---
title: Перечисление конечных точек
description: Получение списка объектов конечной точки.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d8bb01d00fbac03a2b52d95179ec22ca769f9df2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529833"
---
# <a name="list-endpoints"></a><span data-ttu-id="bbfee-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="bbfee-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbfee-104">Получение списка объектов [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="bbfee-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbfee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbfee-105">Permissions</span></span>
<span data-ttu-id="bbfee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbfee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbfee-108">Permission type</span></span>      | <span data-ttu-id="bbfee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbfee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbfee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbfee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbfee-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbfee-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbfee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbfee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbfee-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbfee-113">Not supported.</span></span>    |
|<span data-ttu-id="bbfee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbfee-114">Application</span></span> | <span data-ttu-id="bbfee-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbfee-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbfee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbfee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbfee-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bbfee-117">Optional query parameters</span></span>
<span data-ttu-id="bbfee-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bbfee-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbfee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbfee-119">Request headers</span></span>
| <span data-ttu-id="bbfee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bbfee-120">Name</span></span>      |<span data-ttu-id="bbfee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bbfee-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bbfee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbfee-122">Authorization</span></span>  | <span data-ttu-id="bbfee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbfee-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bbfee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbfee-125">Content-Type</span></span>   | <span data-ttu-id="bbfee-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="bbfee-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbfee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbfee-127">Request body</span></span>
<span data-ttu-id="bbfee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbfee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbfee-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbfee-129">Response</span></span>

<span data-ttu-id="bbfee-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [конечной точки](../resources/endpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbfee-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbfee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bbfee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbfee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbfee-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="bbfee-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbfee-133">Response</span></span>
<span data-ttu-id="bbfee-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbfee-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint",
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
