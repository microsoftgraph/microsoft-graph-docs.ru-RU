---
title: Создание reviewSet
description: Создайте набор отзывов об обнаружении электронных обнаружений.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ef13c35d3450cfd7f409a59a543662ffeb5db0e5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044734"
---
# <a name="create-reviewset"></a><span data-ttu-id="7477d-103">Создание reviewSet</span><span class="sxs-lookup"><span data-stu-id="7477d-103">Create reviewSet</span></span>

<span data-ttu-id="7477d-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7477d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7477d-105">Создайте новый [объект reviewSet.](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="7477d-105">Create a new [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span> <span data-ttu-id="7477d-106">В теле запроса содержится отображаемое имя набора отзывов, которое является единственным рукописным свойством.</span><span class="sxs-lookup"><span data-stu-id="7477d-106">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7477d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7477d-107">Permissions</span></span>

<span data-ttu-id="7477d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7477d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7477d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7477d-110">Permission type</span></span>|<span data-ttu-id="7477d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7477d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7477d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7477d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7477d-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7477d-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7477d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7477d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7477d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7477d-115">Not supported.</span></span>|
|<span data-ttu-id="7477d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7477d-116">Application</span></span>|<span data-ttu-id="7477d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7477d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7477d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7477d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="7477d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7477d-119">Request headers</span></span>

| <span data-ttu-id="7477d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7477d-120">Name</span></span>       | <span data-ttu-id="7477d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7477d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7477d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7477d-122">Authorization</span></span> | <span data-ttu-id="7477d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7477d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7477d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7477d-125">Request body</span></span>

<span data-ttu-id="7477d-126">В теле запроса поставляем представление JSON в [reviewSet](../resources/ediscovery-reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="7477d-126">In the request body, supply JSON representation of the [reviewSet](../resources/ediscovery-reviewset.md).</span></span>  <span data-ttu-id="7477d-127">В следующей таблице перечислены необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="7477d-127">The following table lists the required properties.</span></span>

| <span data-ttu-id="7477d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7477d-128">Property</span></span>     | <span data-ttu-id="7477d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7477d-129">Type</span></span>        | <span data-ttu-id="7477d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7477d-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7477d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="7477d-131">displayName</span></span>  | <span data-ttu-id="7477d-132">string</span><span class="sxs-lookup"><span data-stu-id="7477d-132">string</span></span>      | <span data-ttu-id="7477d-133">Имя набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="7477d-133">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="7477d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477d-134">Response</span></span>

<span data-ttu-id="7477d-135">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7477d-135">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7477d-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="7477d-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7477d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477d-137">Request</span></span>

<span data-ttu-id="7477d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477d-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7477d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7477d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```
# <a name="c"></a>[<span data-ttu-id="7477d-140">C#</span><span class="sxs-lookup"><span data-stu-id="7477d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7477d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7477d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7477d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7477d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7477d-143">Java</span><span class="sxs-lookup"><span data-stu-id="7477d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7477d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477d-144">Response</span></span>

<span data-ttu-id="7477d-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7477d-145">The following is an example of the response.</span></span>

> <span data-ttu-id="7477d-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7477d-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


