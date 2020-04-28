---
title: Удаление Акцесспаккажеассигнментполици
description: Удаление Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74d3416fbffe95d558f75c00bf55ef60523cb3c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448475"
---
# <a name="delete-accesspackageassignmentpolicy"></a><span data-ttu-id="c13a9-103">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="c13a9-103">Delete accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="c13a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13a9-105">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)удалите [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c13a9-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), delete an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c13a9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c13a9-106">Permissions</span></span>

<span data-ttu-id="c13a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c13a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c13a9-109">Permission type</span></span>                        | <span data-ttu-id="c13a9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c13a9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c13a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c13a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c13a9-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13a9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c13a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c13a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13a9-114">Not supported.</span></span> |
| <span data-ttu-id="c13a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c13a9-115">Application</span></span>                            | <span data-ttu-id="c13a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13a9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c13a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c13a9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c13a9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c13a9-118">Request headers</span></span>

| <span data-ttu-id="c13a9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c13a9-119">Name</span></span>          | <span data-ttu-id="c13a9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c13a9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c13a9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c13a9-121">Authorization</span></span> | <span data-ttu-id="c13a9-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="c13a9-122">Bearer \{token\}.</span></span> <span data-ttu-id="c13a9-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c13a9-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c13a9-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c13a9-124">Request body</span></span>

<span data-ttu-id="c13a9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c13a9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c13a9-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c13a9-126">Response</span></span>

<span data-ttu-id="c13a9-127">В случае успешного выполнения этот метод возвращает код ответа "нет содержимого" (204).</span><span class="sxs-lookup"><span data-stu-id="c13a9-127">If successful, this method returns a 204 No Content response code.</span></span> <span data-ttu-id="c13a9-128">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c13a9-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c13a9-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c13a9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c13a9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c13a9-130">Request</span></span>

<span data-ttu-id="c13a9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c13a9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="c13a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="c13a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c13a9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c13a9-136">Response</span></span>

<span data-ttu-id="c13a9-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c13a9-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
