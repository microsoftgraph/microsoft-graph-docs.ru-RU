---
title: Обновление approvalStep
description: Применить утверждение или отказ в принятии решения по объекту approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0fe071b58709a7816a4ffd9c82627542c1905243
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048045"
---
# <a name="update-approvalstep"></a><span data-ttu-id="059ac-103">Обновление approvalStep</span><span class="sxs-lookup"><span data-stu-id="059ac-103">Update approvalStep</span></span>

<span data-ttu-id="059ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="059ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="059ac-105">Применить утверждение или отказ в принятии решения по [объекту approvalStep.](../resources/approvalStep.md)</span><span class="sxs-lookup"><span data-stu-id="059ac-105">Apply approve or deny decision on an [approvalStep](../resources/approvalStep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="059ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="059ac-106">Permissions</span></span>

<span data-ttu-id="059ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="059ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="059ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="059ac-109">Permission type</span></span>                        | <span data-ttu-id="059ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="059ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="059ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="059ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="059ac-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="059ac-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="059ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="059ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="059ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059ac-114">Not supported.</span></span> |
| <span data-ttu-id="059ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="059ac-115">Application</span></span>                            | <span data-ttu-id="059ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059ac-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="059ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="059ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="059ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="059ac-118">Request headers</span></span>

| <span data-ttu-id="059ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="059ac-119">Name</span></span>      |<span data-ttu-id="059ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="059ac-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="059ac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="059ac-121">Authorization</span></span> | <span data-ttu-id="059ac-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="059ac-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="059ac-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="059ac-124">Request body</span></span>

<span data-ttu-id="059ac-125">В следующей таблице показаны свойства, необходимые для этого метода.</span><span class="sxs-lookup"><span data-stu-id="059ac-125">The following table shows the properties that are required for this method.</span></span>

| <span data-ttu-id="059ac-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="059ac-126">Property</span></span>       | <span data-ttu-id="059ac-127">Тип</span><span class="sxs-lookup"><span data-stu-id="059ac-127">Type</span></span>    |<span data-ttu-id="059ac-128">Описание</span><span class="sxs-lookup"><span data-stu-id="059ac-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="059ac-129">reviewResult</span><span class="sxs-lookup"><span data-stu-id="059ac-129">reviewResult</span></span> | <span data-ttu-id="059ac-130">String</span><span class="sxs-lookup"><span data-stu-id="059ac-130">String</span></span> | <span data-ttu-id="059ac-131">Решение утвержденного.</span><span class="sxs-lookup"><span data-stu-id="059ac-131">Decision of the approver.</span></span> <span data-ttu-id="059ac-132">Возможные значения: `Approve`, `Deny`.</span><span class="sxs-lookup"><span data-stu-id="059ac-132">Possible values are: `Approve`, `Deny`.</span></span>|
| <span data-ttu-id="059ac-133">обоснование</span><span class="sxs-lookup"><span data-stu-id="059ac-133">justification</span></span> | <span data-ttu-id="059ac-134">String</span><span class="sxs-lookup"><span data-stu-id="059ac-134">String</span></span> | <span data-ttu-id="059ac-135">Обоснование, связанное с решением утвержденного.</span><span class="sxs-lookup"><span data-stu-id="059ac-135">Justification related to the approver's decision.</span></span> |


## <a name="response"></a><span data-ttu-id="059ac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="059ac-136">Response</span></span>

<span data-ttu-id="059ac-137">В случае успешной работы этот метод возвращает код `204 No Content` ответа в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="059ac-137">If successful, this method returns a `204 No Content` response code in the response body.</span></span> <span data-ttu-id="059ac-138">Однако если у вызываемого не имеется нужных разрешений, метод возвращает код ответа или если код утверждения не найден, метод `403 Forbidden` `404 Not found` возвращается .</span><span class="sxs-lookup"><span data-stu-id="059ac-138">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`.</span></span> <span data-ttu-id="059ac-139">Если запрос уже утвержден другим утверждением на том же этапе утверждения, метод возвращается `409 Conflict` в органе ответа.</span><span class="sxs-lookup"><span data-stu-id="059ac-139">If the request has already been approved by another approver in the same approval stage, the method returns `409 Conflict` in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="059ac-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="059ac-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="059ac-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="059ac-141">Request</span></span>

<span data-ttu-id="059ac-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="059ac-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="059ac-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="059ac-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[<span data-ttu-id="059ac-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059ac-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="059ac-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="059ac-145">Response</span></span>

<span data-ttu-id="059ac-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="059ac-146">The following is an example of the response.</span></span>

> <span data-ttu-id="059ac-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="059ac-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
