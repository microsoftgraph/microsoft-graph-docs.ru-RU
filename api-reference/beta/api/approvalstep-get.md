---
title: Получить утверждениеStep
description: Извлечение свойств объекта approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f55ead753f23862f48e9c89703cc38010f8fbe99
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048052"
---
# <a name="get-approvalstep"></a><span data-ttu-id="8da82-103">Получить утверждениеStep</span><span class="sxs-lookup"><span data-stu-id="8da82-103">Get approvalStep</span></span>

<span data-ttu-id="8da82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da82-105">Извлечение свойств объекта [approvalStep.](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="8da82-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8da82-106">Permissions</span></span>

<span data-ttu-id="8da82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8da82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8da82-109">Permission type</span></span>                        | <span data-ttu-id="8da82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8da82-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8da82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8da82-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8da82-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da82-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8da82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8da82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da82-114">Not supported.</span></span> |
| <span data-ttu-id="8da82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8da82-115">Application</span></span>                            | <span data-ttu-id="8da82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da82-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8da82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8da82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8da82-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8da82-118">Request headers</span></span>

| <span data-ttu-id="8da82-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8da82-119">Name</span></span>      |<span data-ttu-id="8da82-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8da82-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8da82-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8da82-121">Authorization</span></span> | <span data-ttu-id="8da82-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8da82-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8da82-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8da82-124">Request body</span></span>

<span data-ttu-id="8da82-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8da82-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da82-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da82-126">Response</span></span>

<span data-ttu-id="8da82-127">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект approvalStep](../resources/approvalstep.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8da82-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="8da82-128">Однако если у вызываемого не имеется нужных разрешений, метод возвращает `403 Forbidden` код ответа.</span><span class="sxs-lookup"><span data-stu-id="8da82-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8da82-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8da82-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8da82-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8da82-130">Request</span></span>

<span data-ttu-id="8da82-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8da82-131">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="8da82-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8da82-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="c"></a>[<span data-ttu-id="8da82-133">C#</span><span class="sxs-lookup"><span data-stu-id="8da82-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8da82-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8da82-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8da82-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8da82-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8da82-136">Java</span><span class="sxs-lookup"><span data-stu-id="8da82-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="8da82-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da82-137">Response</span></span>

<span data-ttu-id="8da82-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8da82-138">The following is an example of the response.</span></span>

> <span data-ttu-id="8da82-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8da82-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


