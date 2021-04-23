---
title: Получить утверждение
description: Извлечение свойств объекта утверждения.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 083064a405525a33855340bcf920900e3d70ca91
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961368"
---
# <a name="get-approval"></a><span data-ttu-id="786b3-103">Получить утверждение</span><span class="sxs-lookup"><span data-stu-id="786b3-103">Get approval</span></span>

<span data-ttu-id="786b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786b3-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекает свойства объекта [утверждения.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="786b3-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieves the properties of an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="786b3-106">Этот вызов может быть выполнен одобрением, предоставляя идентификатор запроса назначения пакета [доступа.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="786b3-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="786b3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="786b3-107">Permissions</span></span>

<span data-ttu-id="786b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="786b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="786b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="786b3-110">Permission type</span></span>                        | <span data-ttu-id="786b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="786b3-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="786b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="786b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="786b3-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="786b3-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="786b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="786b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="786b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="786b3-115">Not supported.</span></span> |
| <span data-ttu-id="786b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="786b3-116">Application</span></span>                            | <span data-ttu-id="786b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="786b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="786b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="786b3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="786b3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="786b3-119">Request headers</span></span>

| <span data-ttu-id="786b3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="786b3-120">Name</span></span>      |<span data-ttu-id="786b3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="786b3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="786b3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="786b3-122">Authorization</span></span> | <span data-ttu-id="786b3-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="786b3-123">Bearer \{token\}.</span></span> <span data-ttu-id="786b3-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="786b3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="786b3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="786b3-125">Request body</span></span>

<span data-ttu-id="786b3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="786b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786b3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="786b3-127">Response</span></span>

<span data-ttu-id="786b3-128">В случае успеха этот метод возвращает код ответа и запрашиваемого объекта `200 OK` утверждения в тексте ответа. [](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="786b3-128">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="786b3-129">Однако если у вызываемого не имеется нужных разрешений, метод возвращает `403 Forbidden` код ответа.</span><span class="sxs-lookup"><span data-stu-id="786b3-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="786b3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="786b3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="786b3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="786b3-131">Request</span></span>

<span data-ttu-id="786b3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="786b3-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="786b3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="786b3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
# <a name="c"></a>[<span data-ttu-id="786b3-134">C#</span><span class="sxs-lookup"><span data-stu-id="786b3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="786b3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="786b3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="786b3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786b3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="786b3-137">Java</span><span class="sxs-lookup"><span data-stu-id="786b3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="786b3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="786b3-138">Response</span></span>

<span data-ttu-id="786b3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="786b3-139">The following is an example of the response.</span></span>

> <span data-ttu-id="786b3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="786b3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approval"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "abd306ef-f7b2-4a10-9fd1-493454322489",
    "steps": [
        {
            "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
            "displayName": null,
            "reviewedDateTime": null,
            "reviewResult": "NotReviewed",
            "status": "InProgress",
            "assignedToMe": true,
            "justification": "",
            "reviewedBy": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


