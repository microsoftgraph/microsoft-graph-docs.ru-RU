---
title: Перечисление соединителей
description: Получение списка объектов Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b72968bc9404e0936219cb96dfd33467784024e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957477"
---
# <a name="list-connectors"></a><span data-ttu-id="e7dc4-103">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="e7dc4-103">List connectors</span></span>

<span data-ttu-id="e7dc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7dc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7dc4-105">Получение списка объектов [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="e7dc4-105">Retrieve a list of [connector](../resources/connector.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7dc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7dc4-106">Permissions</span></span>
<span data-ttu-id="e7dc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7dc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7dc4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7dc4-109">Permission type</span></span>      | <span data-ttu-id="e7dc4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7dc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7dc4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7dc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7dc4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7dc4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7dc4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7dc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7dc4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-114">Not supported.</span></span>    |
|<span data-ttu-id="e7dc4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7dc4-115">Application</span></span> | <span data-ttu-id="e7dc4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7dc4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7dc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7dc4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e7dc4-118">Optional query parameters</span></span>
<span data-ttu-id="e7dc4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7dc4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7dc4-120">Request headers</span></span>
| <span data-ttu-id="e7dc4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e7dc4-121">Name</span></span>      |<span data-ttu-id="e7dc4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e7dc4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7dc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7dc4-123">Authorization</span></span>  | <span data-ttu-id="e7dc4-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-124">Bearer.</span></span> <span data-ttu-id="e7dc4-125">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e7dc4-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7dc4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7dc4-126">Request body</span></span>
<span data-ttu-id="e7dc4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7dc4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7dc4-128">Response</span></span>

<span data-ttu-id="e7dc4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7dc4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e7dc4-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e7dc4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7dc4-131">Request</span></span>
<span data-ttu-id="e7dc4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7dc4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7dc4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```
# <a name="c"></a>[<span data-ttu-id="e7dc4-134">C#</span><span class="sxs-lookup"><span data-stu-id="e7dc4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7dc4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7dc4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7dc4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7dc4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7dc4-137">Java</span><span class="sxs-lookup"><span data-stu-id="e7dc4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7dc4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7dc4-138">Response</span></span>
<span data-ttu-id="e7dc4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-139">The following is an example of the response.</span></span> <span data-ttu-id="e7dc4-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e7dc4-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7dc4-141">All of the properties will be returned from an actual call.</span></span>
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
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
