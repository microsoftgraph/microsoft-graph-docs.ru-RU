---
title: Удаление Пермиссионгрантполици
description: Удаление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 3a554e5e8a68e30937911159ec8c0498ade41dcc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977954"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="cca1f-103">Удаление Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="cca1f-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="cca1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cca1f-105">Удаление объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cca1f-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cca1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cca1f-106">Permissions</span></span>

<span data-ttu-id="cca1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cca1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cca1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cca1f-109">Permission type</span></span>                        | <span data-ttu-id="cca1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cca1f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cca1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cca1f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cca1f-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cca1f-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="cca1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cca1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cca1f-114">Not supported.</span></span> |
| <span data-ttu-id="cca1f-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cca1f-115">Application</span></span>                            | <span data-ttu-id="cca1f-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cca1f-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="cca1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cca1f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cca1f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cca1f-118">Request headers</span></span>

| <span data-ttu-id="cca1f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cca1f-119">Name</span></span>           | <span data-ttu-id="cca1f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cca1f-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="cca1f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cca1f-121">Authorization</span></span>  | <span data-ttu-id="cca1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cca1f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cca1f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cca1f-124">Request body</span></span>

<span data-ttu-id="cca1f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cca1f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca1f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca1f-126">Response</span></span>

<span data-ttu-id="cca1f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cca1f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cca1f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="cca1f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cca1f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cca1f-130">Request</span></span>

<span data-ttu-id="cca1f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cca1f-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cca1f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cca1f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
```
# <a name="c"></a>[<span data-ttu-id="cca1f-133">C#</span><span class="sxs-lookup"><span data-stu-id="cca1f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cca1f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cca1f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cca1f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cca1f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cca1f-136">Java</span><span class="sxs-lookup"><span data-stu-id="cca1f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cca1f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca1f-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
