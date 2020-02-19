---
title: Список Акцесспаккажеассигнментрекуестс
description: Получение списка объектов Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 24536f48f790413adebb4ab1bfac7cf2de438f45
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108415"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="bc5af-103">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="bc5af-103">List accessPackageAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5af-104">Получение списка объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="bc5af-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="bc5af-105">Полученный список включает все запросы на начисление, текущие и срок действия которых просрочены, которые вызывающий абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="bc5af-105">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc5af-106">Permissions</span></span>

<span data-ttu-id="bc5af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc5af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc5af-109">Permission type</span></span>                        | <span data-ttu-id="bc5af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc5af-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bc5af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc5af-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc5af-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc5af-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="bc5af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc5af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc5af-114">Not supported.</span></span> |
| <span data-ttu-id="bc5af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc5af-115">Application</span></span>                            | <span data-ttu-id="bc5af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc5af-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc5af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc5af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc5af-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc5af-118">Optional query parameters</span></span>

<span data-ttu-id="bc5af-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc5af-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bc5af-120">Например, чтобы получить пакет доступа для каждого запроса, включите `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="bc5af-120">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="bc5af-121">Чтобы получить только запросы для определенного пакета доступа, включите в запрос фильтр, например `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span><span class="sxs-lookup"><span data-stu-id="bc5af-121">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>
<span data-ttu-id="bc5af-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bc5af-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc5af-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc5af-123">Request headers</span></span>

| <span data-ttu-id="bc5af-124">Имя</span><span class="sxs-lookup"><span data-stu-id="bc5af-124">Name</span></span>      |<span data-ttu-id="bc5af-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bc5af-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc5af-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc5af-126">Authorization</span></span> | <span data-ttu-id="bc5af-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="bc5af-127">Bearer \{token\}.</span></span> <span data-ttu-id="bc5af-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="bc5af-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc5af-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc5af-129">Request body</span></span>

<span data-ttu-id="bc5af-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc5af-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc5af-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc5af-131">Response</span></span>

<span data-ttu-id="bc5af-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc5af-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc5af-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="bc5af-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc5af-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc5af-134">Request</span></span>

<span data-ttu-id="bc5af-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc5af-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc5af-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5af-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="bc5af-137">C#</span><span class="sxs-lookup"><span data-stu-id="bc5af-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc5af-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc5af-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc5af-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc5af-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc5af-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc5af-140">Response</span></span>

<span data-ttu-id="bc5af-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc5af-141">The following is an example of the response.</span></span>

> <span data-ttu-id="bc5af-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc5af-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
