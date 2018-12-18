---
title: Список конечных точек
description: Получение списка объектов конечной точки.
author: dkershaw10
ms.openlocfilehash: d455cb8a5d1fb07a3d97cea376d9e2e49266892d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315948"
---
# <a name="list-endpoints"></a><span data-ttu-id="0d2e8-103">Список конечных точек</span><span class="sxs-lookup"><span data-stu-id="0d2e8-103">List endpoints</span></span>

> <span data-ttu-id="0d2e8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d2e8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d2e8-106">Получение списка объектов [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="0d2e8-106">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d2e8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2e8-107">Permissions</span></span>
<span data-ttu-id="0d2e8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d2e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2e8-110">Permission type</span></span>      | <span data-ttu-id="0d2e8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d2e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d2e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2e8-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2e8-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d2e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d2e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-115">Not supported.</span></span>    |
|<span data-ttu-id="0d2e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d2e8-116">Application</span></span> | <span data-ttu-id="0d2e8-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2e8-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d2e8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d2e8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0d2e8-119">Optional query parameters</span></span>
<span data-ttu-id="0d2e8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d2e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d2e8-121">Request headers</span></span>
| <span data-ttu-id="0d2e8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0d2e8-122">Name</span></span>      |<span data-ttu-id="0d2e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2e8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d2e8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d2e8-124">Authorization</span></span>  | <span data-ttu-id="0d2e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0d2e8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d2e8-127">Content-Type</span></span>   | <span data-ttu-id="0d2e8-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="0d2e8-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d2e8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d2e8-129">Request body</span></span>
<span data-ttu-id="0d2e8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d2e8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2e8-131">Response</span></span>

<span data-ttu-id="0d2e8-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [конечной точки](../resources/endpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-132">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d2e8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0d2e8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d2e8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d2e8-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="0d2e8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d2e8-135">Response</span></span>
<span data-ttu-id="0d2e8-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d2e8-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->