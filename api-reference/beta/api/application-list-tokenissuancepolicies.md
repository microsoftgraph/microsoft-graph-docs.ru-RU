---
title: Список назначенных ТокениссуанцеполиЦиес
description: Список ТокениссуанцеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c39d82332e2ea278afd169f059e642c66c59bdc
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142289"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="069fa-103">Список назначенных ТокениссуанцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="069fa-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="069fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="069fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="069fa-105">Перечисление объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="069fa-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="069fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="069fa-106">Permissions</span></span>

<span data-ttu-id="069fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="069fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="069fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="069fa-109">Permission type</span></span>                        | <span data-ttu-id="069fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="069fa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="069fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="069fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="069fa-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="069fa-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="069fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="069fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="069fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="069fa-114">Not supported.</span></span> |
| <span data-ttu-id="069fa-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="069fa-115">Application</span></span>                            | <span data-ttu-id="069fa-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="069fa-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="069fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="069fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="069fa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="069fa-118">Request headers</span></span>

| <span data-ttu-id="069fa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="069fa-119">Name</span></span>          | <span data-ttu-id="069fa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="069fa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="069fa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="069fa-121">Authorization</span></span> | <span data-ttu-id="069fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="069fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="069fa-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="069fa-124">Request body</span></span>

<span data-ttu-id="069fa-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="069fa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="069fa-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="069fa-126">Response</span></span>

<span data-ttu-id="069fa-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="069fa-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="069fa-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="069fa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="069fa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="069fa-129">Request</span></span>

<span data-ttu-id="069fa-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="069fa-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="069fa-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="069fa-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="069fa-132">C#</span><span class="sxs-lookup"><span data-stu-id="069fa-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="069fa-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="069fa-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="069fa-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="069fa-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="069fa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="069fa-135">Response</span></span>

<span data-ttu-id="069fa-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="069fa-136">The following is an example of the response.</span></span>

> <span data-ttu-id="069fa-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="069fa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
