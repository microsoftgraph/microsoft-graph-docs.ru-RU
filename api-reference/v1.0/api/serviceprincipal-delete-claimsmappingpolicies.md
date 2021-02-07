---
title: Удаление типа ресурса claimsMappingPolicy
description: Удалите claimsMappingPolicy из servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d692fb399f6ef0deaaf77070bcb5ebe48ce2818a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132267"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="1bd24-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1bd24-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="1bd24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bd24-105">Удалите [claimsMappingPolicy](../resources/claimsmappingpolicy.md) из [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="1bd24-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bd24-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd24-106">Permissions</span></span>

<span data-ttu-id="1bd24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bd24-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd24-109">Permission type</span></span>                        | <span data-ttu-id="1bd24-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bd24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1bd24-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bd24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bd24-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd24-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="1bd24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bd24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd24-114">Not supported.</span></span> |
| <span data-ttu-id="1bd24-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bd24-115">Application</span></span>                            | <span data-ttu-id="1bd24-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd24-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bd24-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bd24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1bd24-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bd24-118">Request headers</span></span>

| <span data-ttu-id="1bd24-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1bd24-119">Name</span></span>          | <span data-ttu-id="1bd24-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd24-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1bd24-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bd24-121">Authorization</span></span> | <span data-ttu-id="1bd24-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd24-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bd24-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bd24-124">Request body</span></span>

<span data-ttu-id="1bd24-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bd24-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd24-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd24-126">Response</span></span>

<span data-ttu-id="1bd24-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1bd24-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1bd24-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bd24-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1bd24-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bd24-129">Request</span></span>

<span data-ttu-id="1bd24-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bd24-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1bd24-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd24-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="1bd24-132">C#</span><span class="sxs-lookup"><span data-stu-id="1bd24-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bd24-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bd24-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bd24-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bd24-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bd24-135">Java</span><span class="sxs-lookup"><span data-stu-id="1bd24-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1bd24-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd24-136">Response</span></span>

<span data-ttu-id="1bd24-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bd24-137">The following is an example of the response.</span></span>

> <span data-ttu-id="1bd24-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bd24-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

