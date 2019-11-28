---
title: Обновление Кондитионалакцессполици
description: Обновление свойств объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b55e492f7fae576c9026588205eae2bafa99c178
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636766"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="e0d15-103">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="e0d15-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0d15-104">Обновление свойств объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e0d15-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0d15-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0d15-105">Permissions</span></span>

<span data-ttu-id="e0d15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0d15-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0d15-108">Permission type</span></span>                        | <span data-ttu-id="e0d15-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0d15-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="e0d15-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0d15-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0d15-111">Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e0d15-111">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="e0d15-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0d15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0d15-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0d15-113">Not supported.</span></span> |
|<span data-ttu-id="e0d15-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0d15-114">Application</span></span>                            | <span data-ttu-id="e0d15-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0d15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0d15-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0d15-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0d15-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0d15-117">Request headers</span></span>

| <span data-ttu-id="e0d15-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e0d15-118">Name</span></span>          | <span data-ttu-id="e0d15-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e0d15-119">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="e0d15-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0d15-120">Authorization</span></span> | <span data-ttu-id="e0d15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0d15-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e0d15-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0d15-123">Content-Type</span></span>  | <span data-ttu-id="e0d15-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0d15-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0d15-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0d15-126">Request body</span></span>

<span data-ttu-id="e0d15-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e0d15-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e0d15-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e0d15-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e0d15-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e0d15-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="e0d15-130">Список свойств приведен в разделе [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e0d15-130">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="e0d15-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0d15-131">Response</span></span>

<span data-ttu-id="e0d15-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0d15-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0d15-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0d15-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0d15-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0d15-135">Request</span></span>

<span data-ttu-id="e0d15-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0d15-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0d15-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0d15-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
Content-type: application/json

{
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium",
            "low",
        ]
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0d15-138">C#</span><span class="sxs-lookup"><span data-stu-id="e0d15-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0d15-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0d15-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0d15-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0d15-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0d15-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0d15-141">Response</span></span>

<span data-ttu-id="e0d15-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e0d15-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conditionalaccesspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
