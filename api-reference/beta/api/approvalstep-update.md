---
title: Обновление approvalStep
description: Применить утверждение или отказ в принятии решения по объекту approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b8ef436a9319e7a670e0aa5bdc728b39b53c2709
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942524"
---
# <a name="update-approvalstep"></a><span data-ttu-id="a5f46-103">Обновление approvalStep</span><span class="sxs-lookup"><span data-stu-id="a5f46-103">Update approvalStep</span></span>

<span data-ttu-id="a5f46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f46-105">Применить утверждение или отказ в принятии решения по [объекту approvalStep.](../resources/approvalStep.md)</span><span class="sxs-lookup"><span data-stu-id="a5f46-105">Apply approve or deny decision on an [approvalStep](../resources/approvalStep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5f46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f46-106">Permissions</span></span>

<span data-ttu-id="a5f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5f46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f46-109">Permission type</span></span>                        | <span data-ttu-id="a5f46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5f46-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5f46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5f46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5f46-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f46-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a5f46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5f46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5f46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f46-114">Not supported.</span></span> |
| <span data-ttu-id="a5f46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5f46-115">Application</span></span>                            | <span data-ttu-id="a5f46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f46-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5f46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5f46-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5f46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5f46-118">Request headers</span></span>

| <span data-ttu-id="a5f46-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a5f46-119">Name</span></span>      |<span data-ttu-id="a5f46-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f46-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5f46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f46-121">Authorization</span></span> | <span data-ttu-id="a5f46-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a5f46-122">Bearer \{token\}.</span></span> <span data-ttu-id="a5f46-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a5f46-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5f46-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5f46-124">Request body</span></span>

<span data-ttu-id="a5f46-125">В следующей таблице показаны свойства, необходимые для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5f46-125">The following table shows the properties that are required for this method.</span></span>

| <span data-ttu-id="a5f46-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5f46-126">Property</span></span>       | <span data-ttu-id="a5f46-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a5f46-127">Type</span></span>    |<span data-ttu-id="a5f46-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f46-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5f46-129">reviewResult</span><span class="sxs-lookup"><span data-stu-id="a5f46-129">reviewResult</span></span> | <span data-ttu-id="a5f46-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a5f46-130">String</span></span> | <span data-ttu-id="a5f46-131">Решение утвержденного.</span><span class="sxs-lookup"><span data-stu-id="a5f46-131">Decision of the approver.</span></span> <span data-ttu-id="a5f46-132">Возможные значения: `Approve`, `Deny`.</span><span class="sxs-lookup"><span data-stu-id="a5f46-132">Possible values are: `Approve`, `Deny`.</span></span>|
| <span data-ttu-id="a5f46-133">обоснование</span><span class="sxs-lookup"><span data-stu-id="a5f46-133">justification</span></span> | <span data-ttu-id="a5f46-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a5f46-134">String</span></span> | <span data-ttu-id="a5f46-135">Обоснование, связанное с решением утвержденного.</span><span class="sxs-lookup"><span data-stu-id="a5f46-135">Justification related to the approver's decision.</span></span> |


## <a name="response"></a><span data-ttu-id="a5f46-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f46-136">Response</span></span>

<span data-ttu-id="a5f46-137">В случае успешной работы этот метод возвращает код `204 No Content` ответа в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5f46-137">If successful, this method returns a `204 No Content` response code in the response body.</span></span> <span data-ttu-id="a5f46-138">Однако если у вызываемого не имеется нужных разрешений, метод возвращает код ответа или если код утверждения не найден, метод `403 Forbidden` `404 Not found` возвращается .</span><span class="sxs-lookup"><span data-stu-id="a5f46-138">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`.</span></span> <span data-ttu-id="a5f46-139">Если запрос уже утвержден другим утверждением на том же этапе утверждения, метод возвращается `409 Conflict` в органе ответа.</span><span class="sxs-lookup"><span data-stu-id="a5f46-139">If the request has already been approved by another approver in the same approval stage, the method returns `409 Conflict` in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5f46-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5f46-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5f46-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5f46-141">Request</span></span>

<span data-ttu-id="a5f46-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5f46-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5f46-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f46-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[<span data-ttu-id="a5f46-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5f46-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="a5f46-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f46-145">Response</span></span>

<span data-ttu-id="a5f46-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5f46-146">The following is an example of the response.</span></span>

> <span data-ttu-id="a5f46-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5f46-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
