---
title: Получение конечной точки
description: Извлечение свойств и связи объекта определенной конечной точки.
localization_priority: Normal
ms.openlocfilehash: 7c5b7bd28b06e20dbc92b09ff961214828749999
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640429"
---
# <a name="get-endpoint"></a><span data-ttu-id="723a4-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="723a4-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="723a4-104">Извлечение свойств и связи объекта определенного [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="723a4-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="723a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="723a4-105">Permissions</span></span>
<span data-ttu-id="723a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="723a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="723a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="723a4-108">Permission type</span></span>      | <span data-ttu-id="723a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="723a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="723a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="723a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="723a4-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723a4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="723a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="723a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="723a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="723a4-113">Not supported.</span></span>    |
|<span data-ttu-id="723a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="723a4-114">Application</span></span> | <span data-ttu-id="723a4-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723a4-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="723a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="723a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="723a4-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="723a4-117">Optional query parameters</span></span>
<span data-ttu-id="723a4-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="723a4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="723a4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="723a4-119">Request headers</span></span>
| <span data-ttu-id="723a4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="723a4-120">Name</span></span>      |<span data-ttu-id="723a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="723a4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="723a4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="723a4-122">Authorization</span></span>  | <span data-ttu-id="723a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="723a4-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="723a4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="723a4-125">Content-Type</span></span>   | <span data-ttu-id="723a4-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="723a4-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="723a4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="723a4-127">Request body</span></span>
<span data-ttu-id="723a4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="723a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="723a4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="723a4-129">Response</span></span>

<span data-ttu-id="723a4-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [конечной точки](../resources/endpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="723a4-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="723a4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="723a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="723a4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="723a4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="723a4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="723a4-133">Response</span></span>
<span data-ttu-id="723a4-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="723a4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
