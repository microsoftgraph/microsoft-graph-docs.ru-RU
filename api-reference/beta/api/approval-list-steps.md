---
title: Утверждение спискаSteps
description: Список действий по утверждению, связанных с объектом утверждения.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8eda9d7e1524f0dbdbe727d4123f448b6375e585
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048059"
---
# <a name="list-approvalsteps"></a><span data-ttu-id="afd0c-103">Утверждение спискаSteps</span><span class="sxs-lookup"><span data-stu-id="afd0c-103">List approvalSteps</span></span>

<span data-ttu-id="afd0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afd0c-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)перечислены [объекты approvalStep,](../resources/approvalstep.md) связанные с объектом [утверждения.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="afd0c-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), lists the [approvalStep](../resources/approvalstep.md) objects associated with an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="afd0c-106">Этот вызов может быть выполнен одобрением, предоставляя идентификатор запроса назначения пакета [доступа.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="afd0c-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="afd0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afd0c-107">Permissions</span></span>

<span data-ttu-id="afd0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afd0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afd0c-110">Permission type</span></span>                        | <span data-ttu-id="afd0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afd0c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afd0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afd0c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="afd0c-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd0c-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="afd0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afd0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afd0c-115">Not supported.</span></span> |
| <span data-ttu-id="afd0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afd0c-116">Application</span></span>                            | <span data-ttu-id="afd0c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afd0c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afd0c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps
```

## <a name="request-headers"></a><span data-ttu-id="afd0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afd0c-119">Request headers</span></span>

| <span data-ttu-id="afd0c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="afd0c-120">Name</span></span>      |<span data-ttu-id="afd0c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="afd0c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afd0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afd0c-122">Authorization</span></span> | <span data-ttu-id="afd0c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afd0c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd0c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afd0c-125">Request body</span></span>

<span data-ttu-id="afd0c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afd0c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd0c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd0c-127">Response</span></span>

<span data-ttu-id="afd0c-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [approvalStep](../resources/approvalstep.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="afd0c-128">If successful, this method returns a `200 OK` response code and a collection of the [approvalStep](../resources/approvalstep.md) objects in the response body.</span></span> <span data-ttu-id="afd0c-129">Однако если у вызываемого не имеется нужных разрешений, метод возвращает `403 Forbidden` код ответа.</span><span class="sxs-lookup"><span data-stu-id="afd0c-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="afd0c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="afd0c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afd0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd0c-131">Request</span></span>

<span data-ttu-id="afd0c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afd0c-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="afd0c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd0c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps
```
# <a name="c"></a>[<span data-ttu-id="afd0c-134">C#</span><span class="sxs-lookup"><span data-stu-id="afd0c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd0c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd0c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd0c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd0c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd0c-137">Java</span><span class="sxs-lookup"><span data-stu-id="afd0c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="afd0c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd0c-138">Response</span></span>

<span data-ttu-id="afd0c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="afd0c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="afd0c-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="afd0c-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
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
  "description": "List approvalstep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


