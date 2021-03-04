---
title: Удаление connectedOrganization
description: Удаление connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a14207407d3810e53a1b6be871060e8e6f609c8c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437508"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="03bd1-103">Удаление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="03bd1-103">Delete connectedOrganization</span></span>

<span data-ttu-id="03bd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03bd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03bd1-105">Удаление [объекта connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="03bd1-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03bd1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03bd1-106">Permissions</span></span>

<span data-ttu-id="03bd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03bd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bd1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03bd1-109">Permission type</span></span>|<span data-ttu-id="03bd1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03bd1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="03bd1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03bd1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03bd1-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bd1-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="03bd1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03bd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03bd1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03bd1-114">Not supported.</span></span> |
| <span data-ttu-id="03bd1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="03bd1-115">Application</span></span>                            | <span data-ttu-id="03bd1-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bd1-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03bd1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03bd1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03bd1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03bd1-118">Request headers</span></span>
|<span data-ttu-id="03bd1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="03bd1-119">Name</span></span>|<span data-ttu-id="03bd1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="03bd1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03bd1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03bd1-121">Authorization</span></span>|<span data-ttu-id="03bd1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03bd1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03bd1-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03bd1-124">Request body</span></span>
<span data-ttu-id="03bd1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03bd1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03bd1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="03bd1-126">Response</span></span>

<span data-ttu-id="03bd1-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03bd1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="03bd1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="03bd1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03bd1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="03bd1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03bd1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="03bd1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="03bd1-131">C#</span><span class="sxs-lookup"><span data-stu-id="03bd1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03bd1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03bd1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03bd1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03bd1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03bd1-134">Java</span><span class="sxs-lookup"><span data-stu-id="03bd1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="03bd1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03bd1-135">Response</span></span>
<span data-ttu-id="03bd1-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03bd1-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


