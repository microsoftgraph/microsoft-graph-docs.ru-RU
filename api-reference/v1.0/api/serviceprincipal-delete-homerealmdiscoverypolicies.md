---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5d45f7d6dba80b1f36f978181898bef8b7e4a02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013015"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="f1a8a-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a8a-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="f1a8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1a8a-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f1a8a-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a8a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a8a-106">Permissions</span></span>

<span data-ttu-id="f1a8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1a8a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a8a-109">Permission type</span></span>                        | <span data-ttu-id="f1a8a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a8a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1a8a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a8a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1a8a-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f1a8a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="f1a8a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-114">Not supported.</span></span> |
| <span data-ttu-id="f1a8a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a8a-115">Application</span></span>                            | <span data-ttu-id="f1a8a-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f1a8a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a8a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a8a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f1a8a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a8a-118">Request headers</span></span>

| <span data-ttu-id="f1a8a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1a8a-119">Name</span></span>          | <span data-ttu-id="f1a8a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a8a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1a8a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a8a-121">Authorization</span></span> | <span data-ttu-id="f1a8a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a8a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1a8a-124">Request body</span></span>

<span data-ttu-id="f1a8a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1a8a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a8a-126">Response</span></span>

<span data-ttu-id="f1a8a-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f1a8a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1a8a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1a8a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a8a-129">Request</span></span>

<span data-ttu-id="f1a8a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f1a8a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a8a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f1a8a-132">C#</span><span class="sxs-lookup"><span data-stu-id="f1a8a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a8a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a8a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a8a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a8a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1a8a-135">Java</span><span class="sxs-lookup"><span data-stu-id="f1a8a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1a8a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a8a-136">Response</span></span>

<span data-ttu-id="f1a8a-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="f1a8a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a8a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

