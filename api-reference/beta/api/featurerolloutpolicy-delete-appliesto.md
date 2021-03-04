---
title: Удаление appliesTo
description: Удалите directoryObject из выкатки функций.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4bd3ce83f81a040583fdc3400e8ce808e1a3c8f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436134"
---
# <a name="remove-appliesto"></a><span data-ttu-id="888ea-103">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="888ea-103">Remove appliesTo</span></span>

<span data-ttu-id="888ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="888ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="888ea-105">Удалите appliesTo на [объекте featureRolloutPolicy,](../resources/featurerolloutpolicy.md) чтобы удалить [directoryObject](../resources/directoryobject.md) из выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="888ea-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="888ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="888ea-106">Permissions</span></span>

<span data-ttu-id="888ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="888ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="888ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="888ea-109">Permission type</span></span>                        | <span data-ttu-id="888ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="888ea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="888ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="888ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="888ea-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="888ea-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="888ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="888ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="888ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888ea-114">Not supported.</span></span> |
| <span data-ttu-id="888ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="888ea-115">Application</span></span>                            | <span data-ttu-id="888ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="888ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="888ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="888ea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="888ea-118">Request headers</span></span>

| <span data-ttu-id="888ea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="888ea-119">Name</span></span>          | <span data-ttu-id="888ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="888ea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="888ea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="888ea-121">Authorization</span></span> | <span data-ttu-id="888ea-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="888ea-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="888ea-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="888ea-123">Request body</span></span>

<span data-ttu-id="888ea-124">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="888ea-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="888ea-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="888ea-125">Response</span></span>

<span data-ttu-id="888ea-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="888ea-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="888ea-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="888ea-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="888ea-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="888ea-129">Request</span></span>

<span data-ttu-id="888ea-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="888ea-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="888ea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="888ea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="c"></a>[<span data-ttu-id="888ea-132">C#</span><span class="sxs-lookup"><span data-stu-id="888ea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="888ea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="888ea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="888ea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="888ea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="888ea-135">Java</span><span class="sxs-lookup"><span data-stu-id="888ea-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="888ea-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="888ea-136">Response</span></span>

<span data-ttu-id="888ea-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="888ea-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


