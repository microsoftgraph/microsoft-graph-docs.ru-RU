---
title: Список Акцесспаккажересаурцерекуестс
description: Получение списка объектов Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f8e1df84ccb12f4ccdcce3a4aa0e5338be59f3f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951757"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="c0320-103">Список Акцесспаккажересаурцерекуестс</span><span class="sxs-lookup"><span data-stu-id="c0320-103">List accessPackageResourceRequests</span></span>

<span data-ttu-id="c0320-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0320-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0320-105">Получение списка объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c0320-105">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0320-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0320-106">Permissions</span></span>

<span data-ttu-id="c0320-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0320-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0320-109">Permission type</span></span>                        | <span data-ttu-id="c0320-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0320-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0320-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0320-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0320-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c0320-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c0320-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0320-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0320-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0320-114">Not supported.</span></span> |
| <span data-ttu-id="c0320-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0320-115">Application</span></span>                            | <span data-ttu-id="c0320-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0320-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0320-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0320-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0320-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0320-118">Optional query parameters</span></span>

<span data-ttu-id="c0320-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c0320-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0320-120">Например, чтобы получить сведения о том, кто запросил Добавление ресурса в каталог, включите `$expand=requestor` в запрос.</span><span class="sxs-lookup"><span data-stu-id="c0320-120">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="c0320-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c0320-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0320-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0320-122">Request headers</span></span>

| <span data-ttu-id="c0320-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c0320-123">Name</span></span>      |<span data-ttu-id="c0320-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c0320-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0320-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0320-125">Authorization</span></span> | <span data-ttu-id="c0320-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0320-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0320-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0320-128">Request body</span></span>

<span data-ttu-id="c0320-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0320-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0320-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0320-130">Response</span></span>

<span data-ttu-id="c0320-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0320-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0320-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0320-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0320-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0320-133">Request</span></span>

<span data-ttu-id="c0320-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0320-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0320-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0320-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="c"></a>[<span data-ttu-id="c0320-136">C#</span><span class="sxs-lookup"><span data-stu-id="c0320-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0320-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0320-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0320-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0320-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0320-139">Java</span><span class="sxs-lookup"><span data-stu-id="c0320-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0320-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0320-140">Response</span></span>

<span data-ttu-id="c0320-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0320-141">The following is an example of the response.</span></span>

> <span data-ttu-id="c0320-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0320-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


