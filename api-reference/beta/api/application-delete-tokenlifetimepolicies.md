---
title: Удаление типа ресурса tokenLifetimePolicy
description: Удаление Токенлифетимеполици из приложения или servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 73d4b89f8de917937a957dcc6459fe2971342783
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962234"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="4f914-103">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="4f914-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="4f914-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f914-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f914-105">Удаление [токенлифетимеполици](../resources/tokenlifetimepolicy.md) из [приложения](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="4f914-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f914-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f914-106">Permissions</span></span>

<span data-ttu-id="4f914-107">Для вызова этого API требуется один из следующих наборов разрешений.</span><span class="sxs-lookup"><span data-stu-id="4f914-107">One of the following sets of permissions is required to call this API.</span></span> <span data-ttu-id="4f914-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f914-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f914-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f914-109">Permission type</span></span>                        | <span data-ttu-id="4f914-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f914-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f914-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f914-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f914-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4f914-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="4f914-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f914-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f914-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f914-114">Not supported.</span></span> |
| <span data-ttu-id="4f914-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4f914-115">Application</span></span>                            | <span data-ttu-id="4f914-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4f914-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f914-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f914-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="4f914-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f914-118">Request headers</span></span>

| <span data-ttu-id="4f914-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4f914-119">Name</span></span>          | <span data-ttu-id="4f914-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4f914-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f914-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f914-121">Authorization</span></span> | <span data-ttu-id="4f914-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4f914-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f914-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f914-123">Request body</span></span>

<span data-ttu-id="4f914-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f914-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f914-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f914-125">Response</span></span>

<span data-ttu-id="4f914-126">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f914-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4f914-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f914-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f914-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f914-128">Request</span></span>

<span data-ttu-id="4f914-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f914-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f914-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f914-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="4f914-131">C#</span><span class="sxs-lookup"><span data-stu-id="4f914-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f914-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f914-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f914-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f914-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f914-134">Java</span><span class="sxs-lookup"><span data-stu-id="4f914-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f914-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f914-135">Response</span></span>

<span data-ttu-id="4f914-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f914-136">The following is an example of the response.</span></span>

> <span data-ttu-id="4f914-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f914-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


