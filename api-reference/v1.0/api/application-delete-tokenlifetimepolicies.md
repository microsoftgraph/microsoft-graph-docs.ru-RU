---
title: Удаление типа ресурса tokenLifetimePolicy
description: Удалите маркерLifetimePolicy из приложения.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3840de12c08d35629c3d383d3056104d757ce236
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054191"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="2eacd-103">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="2eacd-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="2eacd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eacd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2eacd-105">Удаление [маркераLifetimePolicy](../resources/tokenlifetimepolicy.md) из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="2eacd-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2eacd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2eacd-106">Permissions</span></span>

<span data-ttu-id="2eacd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2eacd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2eacd-109">Permission type</span></span>                        | <span data-ttu-id="2eacd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2eacd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2eacd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2eacd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2eacd-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eacd-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="2eacd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2eacd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eacd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eacd-114">Not supported.</span></span> |
| <span data-ttu-id="2eacd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2eacd-115">Application</span></span>                            | <span data-ttu-id="2eacd-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eacd-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eacd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2eacd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2eacd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2eacd-118">Request headers</span></span>

| <span data-ttu-id="2eacd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2eacd-119">Name</span></span>          | <span data-ttu-id="2eacd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2eacd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2eacd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2eacd-121">Authorization</span></span> | <span data-ttu-id="2eacd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2eacd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2eacd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2eacd-124">Request body</span></span>

<span data-ttu-id="2eacd-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2eacd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eacd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eacd-126">Response</span></span>

<span data-ttu-id="2eacd-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2eacd-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2eacd-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2eacd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2eacd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2eacd-129">Request</span></span>

<span data-ttu-id="2eacd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2eacd-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2eacd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2eacd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="2eacd-132">C#</span><span class="sxs-lookup"><span data-stu-id="2eacd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2eacd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2eacd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2eacd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2eacd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2eacd-135">Java</span><span class="sxs-lookup"><span data-stu-id="2eacd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2eacd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eacd-136">Response</span></span>

<span data-ttu-id="2eacd-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2eacd-137">The following is an example of the response.</span></span>

> <span data-ttu-id="2eacd-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2eacd-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

