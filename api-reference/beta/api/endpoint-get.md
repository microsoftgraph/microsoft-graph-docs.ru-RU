---
title: Получение конечной точки
description: Извлечение свойств и связей определенного конечного объекта.
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: yyuank
ms.openlocfilehash: ab98177176b85101e1122edc52789a7d77d27d15
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760723"
---
# <a name="get-endpoint"></a><span data-ttu-id="60e5c-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="60e5c-103">Get endpoint</span></span>

<span data-ttu-id="60e5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60e5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e5c-105">Извлечение свойств и связей определенного [конечного](../resources/endpoint.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="60e5c-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60e5c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60e5c-106">Permissions</span></span>
<span data-ttu-id="60e5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60e5c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60e5c-109">Permission type</span></span>      | <span data-ttu-id="60e5c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60e5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e5c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60e5c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60e5c-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e5c-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60e5c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60e5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60e5c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e5c-114">Not supported.</span></span>    |
|<span data-ttu-id="60e5c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60e5c-115">Application</span></span> | <span data-ttu-id="60e5c-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e5c-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60e5c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60e5c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60e5c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60e5c-118">Optional query parameters</span></span>
<span data-ttu-id="60e5c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60e5c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60e5c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60e5c-120">Request headers</span></span>
| <span data-ttu-id="60e5c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60e5c-121">Name</span></span>      |<span data-ttu-id="60e5c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60e5c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60e5c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60e5c-123">Authorization</span></span>  | <span data-ttu-id="60e5c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e5c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60e5c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60e5c-126">Request body</span></span>
<span data-ttu-id="60e5c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60e5c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e5c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e5c-128">Response</span></span>

<span data-ttu-id="60e5c-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [Endpoint](../resources/endpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60e5c-129">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60e5c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="60e5c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="60e5c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="60e5c-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="60e5c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="60e5c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="60e5c-133">C#</span><span class="sxs-lookup"><span data-stu-id="60e5c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60e5c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60e5c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60e5c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60e5c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60e5c-136">Java</span><span class="sxs-lookup"><span data-stu-id="60e5c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="60e5c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e5c-137">Response</span></span>
<span data-ttu-id="60e5c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60e5c-138">Here is an example of the response.</span></span>
><span data-ttu-id="60e5c-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60e5c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
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
  ]
}
-->
