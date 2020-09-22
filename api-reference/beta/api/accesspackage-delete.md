---
title: Удаление Акцесспаккаже
description: Удаление Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 008af7b676514cd33da0bd048681810cf4db2973
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972709"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="c220e-103">Удаление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="c220e-103">Delete accessPackage</span></span>

<span data-ttu-id="c220e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c220e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c220e-105">Удаление объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="c220e-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c220e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c220e-106">Permissions</span></span>

<span data-ttu-id="c220e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c220e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c220e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c220e-109">Permission type</span></span>                        | <span data-ttu-id="c220e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c220e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c220e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c220e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c220e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c220e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c220e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c220e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c220e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c220e-114">Not supported.</span></span> |
| <span data-ttu-id="c220e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c220e-115">Application</span></span>                            | <span data-ttu-id="c220e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c220e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c220e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c220e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}

```

## <a name="request-headers"></a><span data-ttu-id="c220e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c220e-118">Request headers</span></span>

| <span data-ttu-id="c220e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c220e-119">Name</span></span>          | <span data-ttu-id="c220e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c220e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c220e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c220e-121">Authorization</span></span> | <span data-ttu-id="c220e-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="c220e-122">Bearer \{token\}.</span></span> <span data-ttu-id="c220e-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c220e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c220e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c220e-124">Request body</span></span>

<span data-ttu-id="c220e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c220e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c220e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c220e-126">Response</span></span>

<span data-ttu-id="c220e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c220e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c220e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c220e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c220e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c220e-130">Request</span></span>

<span data-ttu-id="c220e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c220e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c220e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c220e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="c220e-133">C#</span><span class="sxs-lookup"><span data-stu-id="c220e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c220e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c220e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c220e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c220e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c220e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c220e-136">Response</span></span>

<span data-ttu-id="c220e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c220e-137">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


