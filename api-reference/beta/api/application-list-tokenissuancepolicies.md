---
title: Список назначенных ТокениссуанцеполиЦиес
description: Список ТокениссуанцеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 046690b1ff4f69d54f46bd21ae2bd1c5fe487001
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962065"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="24cde-103">Список назначенных ТокениссуанцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="24cde-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="24cde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24cde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24cde-105">Перечисление объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="24cde-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24cde-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24cde-106">Permissions</span></span>

<span data-ttu-id="24cde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24cde-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24cde-109">Permission type</span></span>                        | <span data-ttu-id="24cde-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24cde-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="24cde-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24cde-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24cde-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24cde-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="24cde-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24cde-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24cde-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cde-114">Not supported.</span></span> |
| <span data-ttu-id="24cde-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="24cde-115">Application</span></span>                            | <span data-ttu-id="24cde-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24cde-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24cde-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24cde-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="24cde-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24cde-118">Request headers</span></span>

| <span data-ttu-id="24cde-119">Имя</span><span class="sxs-lookup"><span data-stu-id="24cde-119">Name</span></span>          | <span data-ttu-id="24cde-120">Описание</span><span class="sxs-lookup"><span data-stu-id="24cde-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24cde-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24cde-121">Authorization</span></span> | <span data-ttu-id="24cde-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24cde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24cde-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24cde-124">Request body</span></span>

<span data-ttu-id="24cde-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24cde-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24cde-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="24cde-126">Response</span></span>

<span data-ttu-id="24cde-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24cde-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24cde-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="24cde-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24cde-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="24cde-129">Request</span></span>

<span data-ttu-id="24cde-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24cde-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="24cde-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="24cde-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="24cde-132">C#</span><span class="sxs-lookup"><span data-stu-id="24cde-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24cde-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24cde-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24cde-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24cde-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24cde-135">Java</span><span class="sxs-lookup"><span data-stu-id="24cde-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenissuancepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24cde-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="24cde-136">Response</span></span>

<span data-ttu-id="24cde-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24cde-137">The following is an example of the response.</span></span>

> <span data-ttu-id="24cde-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24cde-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


