---
title: Список assigned tokenIssuancePolicies
description: Список tokenIssuancePolicies, которые назначены приложению.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 155250bd4b7fb8a163d95eb44d5987c0d0a8d7bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129179"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="29296-103">Список assigned tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="29296-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="29296-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29296-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29296-105">Список объектов [tokenIssuancePolicy,](../resources/tokenissuancepolicy.md) которые назначены [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="29296-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29296-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29296-106">Permissions</span></span>

<span data-ttu-id="29296-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29296-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29296-109">Permission type</span></span>                        | <span data-ttu-id="29296-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29296-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29296-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29296-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29296-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29296-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="29296-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29296-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29296-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29296-114">Not supported.</span></span> |
| <span data-ttu-id="29296-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29296-115">Application</span></span>                            | <span data-ttu-id="29296-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29296-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29296-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29296-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="29296-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29296-118">Request headers</span></span>

| <span data-ttu-id="29296-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29296-119">Name</span></span>          | <span data-ttu-id="29296-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29296-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="29296-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29296-121">Authorization</span></span> | <span data-ttu-id="29296-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29296-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29296-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29296-124">Request body</span></span>

<span data-ttu-id="29296-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29296-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29296-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="29296-126">Response</span></span>

<span data-ttu-id="29296-127">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29296-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29296-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="29296-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29296-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="29296-129">Request</span></span>

<span data-ttu-id="29296-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29296-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="29296-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="29296-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="29296-132">C#</span><span class="sxs-lookup"><span data-stu-id="29296-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29296-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29296-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29296-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29296-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29296-135">Java</span><span class="sxs-lookup"><span data-stu-id="29296-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenissuancepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29296-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="29296-136">Response</span></span>

<span data-ttu-id="29296-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29296-137">The following is an example of the response.</span></span>

> <span data-ttu-id="29296-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29296-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



