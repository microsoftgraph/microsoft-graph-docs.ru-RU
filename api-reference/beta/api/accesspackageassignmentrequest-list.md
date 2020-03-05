---
title: Список Акцесспаккажеассигнментрекуестс
description: Получение списка объектов Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e6b436c59feda5fbb890a5f83cb5d11a3c3dc0de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442056"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="d2634-103">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="d2634-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="d2634-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2634-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2634-105">Получение списка объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="d2634-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="d2634-106">Полученный список включает все запросы на начисление, текущие и срок действия которых просрочены, которые вызывающий абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="d2634-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2634-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2634-107">Permissions</span></span>

<span data-ttu-id="d2634-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2634-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2634-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2634-110">Permission type</span></span>                        | <span data-ttu-id="d2634-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2634-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2634-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2634-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2634-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2634-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d2634-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2634-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2634-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2634-115">Not supported.</span></span> |
| <span data-ttu-id="d2634-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2634-116">Application</span></span>                            | <span data-ttu-id="d2634-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2634-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2634-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2634-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2634-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2634-119">Optional query parameters</span></span>

<span data-ttu-id="d2634-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2634-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d2634-121">Например, чтобы получить пакет доступа для каждого запроса, включите `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="d2634-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="d2634-122">Чтобы получить только запросы для определенного пакета доступа, включите в запрос фильтр, например `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span><span class="sxs-lookup"><span data-stu-id="d2634-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>
<span data-ttu-id="d2634-123">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d2634-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2634-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2634-124">Request headers</span></span>

| <span data-ttu-id="d2634-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d2634-125">Name</span></span>      |<span data-ttu-id="d2634-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d2634-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2634-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2634-127">Authorization</span></span> | <span data-ttu-id="d2634-128">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="d2634-128">Bearer \{token\}.</span></span> <span data-ttu-id="d2634-129">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d2634-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2634-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2634-130">Request body</span></span>

<span data-ttu-id="d2634-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2634-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2634-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2634-132">Response</span></span>

<span data-ttu-id="d2634-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2634-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2634-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2634-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2634-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2634-135">Request</span></span>

<span data-ttu-id="d2634-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2634-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2634-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2634-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="d2634-138">C#</span><span class="sxs-lookup"><span data-stu-id="d2634-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2634-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2634-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2634-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2634-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2634-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2634-141">Response</span></span>

<span data-ttu-id="d2634-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2634-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d2634-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2634-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
