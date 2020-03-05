---
title: Список АкцесспаккажеассигнментполиЦиес
description: Получение списка объектов Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3eeff42ac2de58e2197da4f349b4abf5a9b72c2a
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534409"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="50d58-103">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="50d58-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="50d58-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="50d58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d58-105">Получение списка объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="50d58-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="50d58-106">Полученный список включает все политики назначения, которые абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="50d58-106">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="50d58-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50d58-107">Permissions</span></span>

<span data-ttu-id="50d58-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50d58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50d58-110">Permission type</span></span>                        | <span data-ttu-id="50d58-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50d58-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50d58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50d58-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="50d58-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d58-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="50d58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50d58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50d58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d58-115">Not supported.</span></span> |
| <span data-ttu-id="50d58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50d58-116">Application</span></span>                            | <span data-ttu-id="50d58-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d58-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50d58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50d58-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50d58-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50d58-119">Optional query parameters</span></span>

<span data-ttu-id="50d58-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50d58-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="50d58-121">Например, чтобы получить политику назначения пакетов Access с указанным отображаемым именем, включите `$filter=displayName eq 'Employee sales support'` в запрос.</span><span class="sxs-lookup"><span data-stu-id="50d58-121">For example, to retrieve a access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="50d58-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="50d58-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="50d58-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50d58-123">Request headers</span></span>

| <span data-ttu-id="50d58-124">Имя</span><span class="sxs-lookup"><span data-stu-id="50d58-124">Name</span></span>      |<span data-ttu-id="50d58-125">Описание</span><span class="sxs-lookup"><span data-stu-id="50d58-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50d58-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d58-126">Authorization</span></span> | <span data-ttu-id="50d58-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="50d58-127">Bearer \{token\}.</span></span> <span data-ttu-id="50d58-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="50d58-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50d58-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50d58-129">Request body</span></span>

<span data-ttu-id="50d58-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50d58-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d58-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="50d58-131">Response</span></span>

<span data-ttu-id="50d58-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50d58-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50d58-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="50d58-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50d58-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="50d58-134">Request</span></span>

<span data-ttu-id="50d58-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50d58-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50d58-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="50d58-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="50d58-137">C#</span><span class="sxs-lookup"><span data-stu-id="50d58-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50d58-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50d58-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50d58-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50d58-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50d58-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="50d58-140">Response</span></span>

<span data-ttu-id="50d58-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50d58-141">The following is an example of the response.</span></span>

> <span data-ttu-id="50d58-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50d58-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
