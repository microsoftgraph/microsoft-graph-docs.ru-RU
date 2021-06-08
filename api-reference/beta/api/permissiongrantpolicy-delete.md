---
title: Удаление permissionGrantPolicy
description: Удаление объекта permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 9495685dda154160176279e769b3bcbae7bae0e6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787690"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="96cbb-103">Удаление permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="96cbb-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="96cbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96cbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96cbb-105">Удаление [объекта permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96cbb-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96cbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96cbb-106">Permissions</span></span>

<span data-ttu-id="96cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96cbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96cbb-109">Permission type</span></span>                        | <span data-ttu-id="96cbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96cbb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96cbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96cbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96cbb-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96cbb-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="96cbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96cbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96cbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96cbb-114">Not supported.</span></span> |
| <span data-ttu-id="96cbb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="96cbb-115">Application</span></span>                            | <span data-ttu-id="96cbb-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96cbb-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="96cbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96cbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96cbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96cbb-118">Request headers</span></span>

| <span data-ttu-id="96cbb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="96cbb-119">Name</span></span>           | <span data-ttu-id="96cbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96cbb-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="96cbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96cbb-121">Authorization</span></span>  | <span data-ttu-id="96cbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96cbb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96cbb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96cbb-124">Request body</span></span>

<span data-ttu-id="96cbb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96cbb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96cbb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="96cbb-126">Response</span></span>

<span data-ttu-id="96cbb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96cbb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96cbb-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="96cbb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96cbb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="96cbb-130">Request</span></span>

<span data-ttu-id="96cbb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96cbb-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96cbb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="96cbb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
```
# <a name="c"></a>[<span data-ttu-id="96cbb-133">C#</span><span class="sxs-lookup"><span data-stu-id="96cbb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96cbb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96cbb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96cbb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96cbb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96cbb-136">Java</span><span class="sxs-lookup"><span data-stu-id="96cbb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96cbb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="96cbb-137">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
