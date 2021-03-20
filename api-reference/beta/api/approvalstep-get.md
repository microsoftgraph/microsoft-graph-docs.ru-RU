---
title: Получить утверждениеStep
description: Извлечение свойств объекта approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7cc5d37c5dea66bc90661bf23b75ea43d82bc82e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942546"
---
# <a name="get-approvalstep"></a><span data-ttu-id="aaa92-103">Получить утверждениеStep</span><span class="sxs-lookup"><span data-stu-id="aaa92-103">Get approvalStep</span></span>

<span data-ttu-id="aaa92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaa92-105">Извлечение свойств объекта [approvalStep.](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="aaa92-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaa92-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa92-106">Permissions</span></span>

<span data-ttu-id="aaa92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aaa92-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa92-109">Permission type</span></span>                        | <span data-ttu-id="aaa92-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaa92-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aaa92-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaa92-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aaa92-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa92-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="aaa92-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaa92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaa92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa92-114">Not supported.</span></span> |
| <span data-ttu-id="aaa92-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaa92-115">Application</span></span>                            | <span data-ttu-id="aaa92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa92-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaa92-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaa92-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="aaa92-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaa92-118">Request headers</span></span>

| <span data-ttu-id="aaa92-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aaa92-119">Name</span></span>      |<span data-ttu-id="aaa92-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa92-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaa92-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa92-121">Authorization</span></span> | <span data-ttu-id="aaa92-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="aaa92-122">Bearer \{token\}.</span></span> <span data-ttu-id="aaa92-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="aaa92-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaa92-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaa92-124">Request body</span></span>

<span data-ttu-id="aaa92-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaa92-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaa92-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa92-126">Response</span></span>

<span data-ttu-id="aaa92-127">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект approvalStep](../resources/approvalstep.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aaa92-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="aaa92-128">Однако если у вызываемого не имеется нужных разрешений, метод возвращает `403 Forbidden` код ответа.</span><span class="sxs-lookup"><span data-stu-id="aaa92-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="aaa92-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="aaa92-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aaa92-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaa92-130">Request</span></span>

<span data-ttu-id="aaa92-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaa92-131">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="aaa92-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaa92-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="c"></a>[<span data-ttu-id="aaa92-133">C#</span><span class="sxs-lookup"><span data-stu-id="aaa92-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaa92-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaa92-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaa92-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaa92-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaa92-136">Java</span><span class="sxs-lookup"><span data-stu-id="aaa92-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="aaa92-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa92-137">Response</span></span>

<span data-ttu-id="aaa92-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aaa92-138">The following is an example of the response.</span></span>

> <span data-ttu-id="aaa92-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaa92-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


