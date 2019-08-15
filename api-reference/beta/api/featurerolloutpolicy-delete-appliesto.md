---
title: Удаление appliesTo
description: Удаление directoryObject из развертывания компонента.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 020dd8bcd01e78cfe194df148cb57a3307dbe6ed
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419806"
---
# <a name="remove-appliesto"></a><span data-ttu-id="e1a3e-103">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="e1a3e-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a3e-104">Удалите элемент appliesTo в объекте [феатурероллаутполици](../resources/featurerolloutpolicy.md) , чтобы удалить [directoryObject](../resources/directoryobject.md) из развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1a3e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a3e-105">Permissions</span></span>

<span data-ttu-id="e1a3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1a3e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a3e-108">Permission type</span></span>                        | <span data-ttu-id="e1a3e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1a3e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1a3e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1a3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1a3e-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="e1a3e-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="e1a3e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1a3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a3e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-113">Not supported.</span></span> |
| <span data-ttu-id="e1a3e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1a3e-114">Application</span></span>                            | <span data-ttu-id="e1a3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1a3e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1a3e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e1a3e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1a3e-117">Request headers</span></span>

| <span data-ttu-id="e1a3e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e1a3e-118">Name</span></span>          | <span data-ttu-id="e1a3e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a3e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e1a3e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1a3e-120">Authorization</span></span> | <span data-ttu-id="e1a3e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e1a3e-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1a3e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1a3e-122">Request body</span></span>

<span data-ttu-id="e1a3e-123">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1a3e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a3e-124">Response</span></span>

<span data-ttu-id="e1a3e-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1a3e-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1a3e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1a3e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1a3e-128">Request</span></span>

<span data-ttu-id="e1a3e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1a3e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1a3e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1a3e-131">C#</span><span class="sxs-lookup"><span data-stu-id="e1a3e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1a3e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1a3e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1a3e-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1a3e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1a3e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a3e-134">Response</span></span>

<span data-ttu-id="e1a3e-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1a3e-135">The following is an example of the response.</span></span>

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
