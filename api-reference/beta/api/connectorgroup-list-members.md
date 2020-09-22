---
title: Список участников
description: Получение списка объектов Connector, связанных с Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1960f7394e2c1482d334812d390b1b60b07dafd9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996477"
---
# <a name="list-members"></a><span data-ttu-id="bfc3f-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="bfc3f-103">List members</span></span>

<span data-ttu-id="bfc3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfc3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfc3f-105">Получение списка объектов [Connector](../resources/connector.md) , связанных с [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="bfc3f-105">Retrieve a list of [connector](../resources/connector.md) objects associated with a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bfc3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfc3f-106">Permissions</span></span>
<span data-ttu-id="bfc3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfc3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfc3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfc3f-109">Permission type</span></span>      | <span data-ttu-id="bfc3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfc3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfc3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfc3f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfc3f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfc3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfc3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-114">Not supported.</span></span>    |
|<span data-ttu-id="bfc3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfc3f-115">Application</span></span> | <span data-ttu-id="bfc3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bfc3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfc3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfc3f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfc3f-118">Optional query parameters</span></span>
<span data-ttu-id="bfc3f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfc3f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfc3f-120">Request headers</span></span>
| <span data-ttu-id="bfc3f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bfc3f-121">Name</span></span>      |<span data-ttu-id="bfc3f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bfc3f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfc3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc3f-123">Authorization</span></span>  | <span data-ttu-id="bfc3f-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-124">Bearer.</span></span> <span data-ttu-id="bfc3f-125">Обязательно</span><span class="sxs-lookup"><span data-stu-id="bfc3f-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfc3f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfc3f-126">Request body</span></span>
<span data-ttu-id="bfc3f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfc3f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfc3f-128">Response</span></span>

<span data-ttu-id="bfc3f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfc3f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bfc3f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bfc3f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfc3f-131">Request</span></span>
<span data-ttu-id="bfc3f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfc3f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfc3f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="bfc3f-134">C#</span><span class="sxs-lookup"><span data-stu-id="bfc3f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfc3f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfc3f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfc3f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfc3f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bfc3f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfc3f-137">Response</span></span>
<span data-ttu-id="bfc3f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-138">The following is an example of the response.</span></span> <span data-ttu-id="bfc3f-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bfc3f-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfc3f-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


