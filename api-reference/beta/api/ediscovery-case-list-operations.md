---
title: Операции списка
description: Получите список caseOperations из объекта case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ee95efa24aa1f7a3c0254e3da2e22cc43e3568c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776685"
---
# <a name="list-operations"></a><span data-ttu-id="8ec38-103">Операции списка</span><span class="sxs-lookup"><span data-stu-id="8ec38-103">List operations</span></span>

<span data-ttu-id="8ec38-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8ec38-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec38-105">Получите список [caseOperations из](../resources/ediscovery-caseoperation.md) [объекта case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="8ec38-105">Get the list of [caseOperations](../resources/ediscovery-caseoperation.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ec38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec38-106">Permissions</span></span>

<span data-ttu-id="8ec38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec38-109">Permission type</span></span>|<span data-ttu-id="8ec38-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ec38-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ec38-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ec38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ec38-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec38-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8ec38-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ec38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ec38-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec38-114">Not supported.</span></span>|
|<span data-ttu-id="8ec38-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ec38-115">Application</span></span>|<span data-ttu-id="8ec38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec38-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ec38-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ec38-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ec38-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8ec38-118">Optional query parameters</span></span>

<span data-ttu-id="8ec38-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8ec38-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8ec38-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8ec38-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ec38-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ec38-121">Request headers</span></span>

|<span data-ttu-id="8ec38-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8ec38-122">Name</span></span>|<span data-ttu-id="8ec38-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec38-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ec38-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ec38-124">Authorization</span></span>|<span data-ttu-id="8ec38-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ec38-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec38-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ec38-127">Request body</span></span>
<span data-ttu-id="8ec38-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ec38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ec38-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec38-129">Response</span></span>

<span data-ttu-id="8ec38-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ec38-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ec38-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ec38-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ec38-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ec38-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8ec38-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ec38-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_caseoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations
```
# <a name="c"></a>[<span data-ttu-id="8ec38-134">C#</span><span class="sxs-lookup"><span data-stu-id="8ec38-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-caseoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ec38-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ec38-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-caseoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ec38-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ec38-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-caseoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ec38-137">Java</span><span class="sxs-lookup"><span data-stu-id="8ec38-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-caseoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ec38-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec38-138">Response</span></span>

<span data-ttu-id="8ec38-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8ec38-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.caseOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
      "id": "41362b70-2b70-4136-702b-3641702b3641",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
