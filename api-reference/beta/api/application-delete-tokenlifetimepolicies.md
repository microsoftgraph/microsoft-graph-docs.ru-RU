---
title: Удаление типа ресурса tokenLifetimePolicy
description: Удаление tokenLifetimePolicy из приложения или servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: efe54936a33c468590bfb31d046b116544a373a5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129242"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="440c5-103">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="440c5-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="440c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="440c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="440c5-105">Удалите [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) из [приложения](../resources/application.md) или [servicePrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="440c5-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="440c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="440c5-106">Permissions</span></span>

<span data-ttu-id="440c5-107">Для вызова этого API требуется один из следующих наборов разрешений.</span><span class="sxs-lookup"><span data-stu-id="440c5-107">One of the following sets of permissions is required to call this API.</span></span> <span data-ttu-id="440c5-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="440c5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="440c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="440c5-109">Permission type</span></span>                        | <span data-ttu-id="440c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="440c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="440c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="440c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="440c5-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="440c5-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="440c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="440c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="440c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="440c5-114">Not supported.</span></span> |
| <span data-ttu-id="440c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="440c5-115">Application</span></span>                            | <span data-ttu-id="440c5-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="440c5-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="440c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="440c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="440c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="440c5-118">Request headers</span></span>

| <span data-ttu-id="440c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="440c5-119">Name</span></span>          | <span data-ttu-id="440c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="440c5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="440c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="440c5-121">Authorization</span></span> | <span data-ttu-id="440c5-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="440c5-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="440c5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="440c5-123">Request body</span></span>

<span data-ttu-id="440c5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="440c5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="440c5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="440c5-125">Response</span></span>

<span data-ttu-id="440c5-126">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="440c5-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="440c5-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="440c5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="440c5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="440c5-128">Request</span></span>

<span data-ttu-id="440c5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="440c5-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="440c5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="440c5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="440c5-131">C#</span><span class="sxs-lookup"><span data-stu-id="440c5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="440c5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="440c5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="440c5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="440c5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="440c5-134">Java</span><span class="sxs-lookup"><span data-stu-id="440c5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="440c5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="440c5-135">Response</span></span>

<span data-ttu-id="440c5-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="440c5-136">The following is an example of the response.</span></span>

> <span data-ttu-id="440c5-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="440c5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



