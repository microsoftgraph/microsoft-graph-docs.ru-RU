---
title: Удаление accessPackage
description: Удаление accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b48b132bc12bd35b248be0efe33b038fcd884a35
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176404"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="a5fbb-103">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="a5fbb-103">Delete accessPackage</span></span>

<span data-ttu-id="a5fbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5fbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5fbb-105">Удаление объекта [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="a5fbb-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5fbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fbb-106">Permissions</span></span>

<span data-ttu-id="a5fbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5fbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fbb-109">Permission type</span></span>                        | <span data-ttu-id="a5fbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5fbb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5fbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5fbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5fbb-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fbb-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a5fbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5fbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5fbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-114">Not supported.</span></span> |
| <span data-ttu-id="a5fbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5fbb-115">Application</span></span>                            | <span data-ttu-id="a5fbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5fbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5fbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5fbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5fbb-118">Request headers</span></span>

| <span data-ttu-id="a5fbb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a5fbb-119">Name</span></span>          | <span data-ttu-id="a5fbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fbb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a5fbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5fbb-121">Authorization</span></span> | <span data-ttu-id="a5fbb-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-122">Bearer \{token\}.</span></span> <span data-ttu-id="a5fbb-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5fbb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5fbb-124">Request body</span></span>

<span data-ttu-id="a5fbb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5fbb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fbb-126">Response</span></span>

<span data-ttu-id="a5fbb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5fbb-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5fbb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5fbb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5fbb-130">Request</span></span>

<span data-ttu-id="a5fbb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5fbb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5fbb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="a5fbb-133">C#</span><span class="sxs-lookup"><span data-stu-id="a5fbb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5fbb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5fbb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5fbb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5fbb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5fbb-136">Java</span><span class="sxs-lookup"><span data-stu-id="a5fbb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5fbb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fbb-137">Response</span></span>

<span data-ttu-id="a5fbb-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5fbb-138">The following is an example of the response.</span></span>

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


