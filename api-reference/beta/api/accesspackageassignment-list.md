---
title: Список Акцесспаккажеассигнментс
description: Получение списка объектов акцесспаккажеассигнмент.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a14bfbdf7785c378a132d308711d4fd21a815413
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108429"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="7a49a-103">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="7a49a-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a49a-104">Получение списка объектов [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="7a49a-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="7a49a-105">В полученном списке содержатся все назначения, текущие и просроченные, которые вызывающий абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="7a49a-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a49a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a49a-106">Permissions</span></span>

<span data-ttu-id="7a49a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a49a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a49a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a49a-109">Permission type</span></span>                        | <span data-ttu-id="7a49a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a49a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a49a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a49a-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="7a49a-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a49a-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7a49a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a49a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a49a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a49a-114">Not supported.</span></span> |
| <span data-ttu-id="7a49a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a49a-115">Application</span></span>                            | <span data-ttu-id="7a49a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a49a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a49a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a49a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a49a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a49a-118">Optional query parameters</span></span>

<span data-ttu-id="7a49a-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a49a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7a49a-120">Например, чтобы возвратить целевой пользователь и пакет Access, включите `$expand=target,accessPackage`.</span><span class="sxs-lookup"><span data-stu-id="7a49a-120">For example, to also return the target user and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="7a49a-121">Чтобы получить только доставленные назначения, можно включить запрос `$filter=assignmentState eq 'Delivered'`.</span><span class="sxs-lookup"><span data-stu-id="7a49a-121">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="7a49a-122">Чтобы получить только назначения для определенного пользователя, можно включить запрос с назначениями, предназначенными для идентификатора объекта этого пользователя `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span><span class="sxs-lookup"><span data-stu-id="7a49a-122">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="7a49a-123">Чтобы получить только назначения для определенного пользователя и определенного пакета Access, можно включить запрос с назначениями, предназначенными для этого пакета доступа, и ИДЕНТИФИКАТОРом объекта этого пользователя `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span><span class="sxs-lookup"><span data-stu-id="7a49a-123">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>

<span data-ttu-id="7a49a-124">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a49a-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a49a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a49a-125">Request headers</span></span>

| <span data-ttu-id="7a49a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="7a49a-126">Name</span></span>      |<span data-ttu-id="7a49a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7a49a-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a49a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a49a-128">Authorization</span></span> | <span data-ttu-id="7a49a-129">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="7a49a-129">Bearer \{token\}.</span></span> <span data-ttu-id="7a49a-130">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="7a49a-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a49a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a49a-131">Request body</span></span>

<span data-ttu-id="7a49a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a49a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a49a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a49a-133">Response</span></span>

<span data-ttu-id="7a49a-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a49a-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a49a-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="7a49a-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a49a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a49a-136">Request</span></span>

<span data-ttu-id="7a49a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a49a-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a49a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a49a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="7a49a-139">C#</span><span class="sxs-lookup"><span data-stu-id="7a49a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a49a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a49a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a49a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a49a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a49a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a49a-142">Response</span></span>

<span data-ttu-id="7a49a-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a49a-143">The following is an example of the response.</span></span>

> <span data-ttu-id="7a49a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a49a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
