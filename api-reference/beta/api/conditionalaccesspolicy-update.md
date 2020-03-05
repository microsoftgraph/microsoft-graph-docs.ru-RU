---
title: Обновление Кондитионалакцессполици
description: Обновление свойств объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7716697d6dd5cdb852c0851c301dba00b28f3fe8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437961"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="45d7b-103">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="45d7b-103">Update conditionalAccessPolicy</span></span>

<span data-ttu-id="45d7b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45d7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45d7b-105">Обновление свойств объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="45d7b-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45d7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45d7b-106">Permissions</span></span>

<span data-ttu-id="45d7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45d7b-109">Permission type</span></span>                        | <span data-ttu-id="45d7b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45d7b-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="45d7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45d7b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45d7b-112">Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="45d7b-112">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="45d7b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45d7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45d7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d7b-114">Not supported.</span></span> |
|<span data-ttu-id="45d7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45d7b-115">Application</span></span>                            | <span data-ttu-id="45d7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d7b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45d7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45d7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45d7b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45d7b-118">Request headers</span></span>

| <span data-ttu-id="45d7b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="45d7b-119">Name</span></span>          | <span data-ttu-id="45d7b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="45d7b-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="45d7b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45d7b-121">Authorization</span></span> | <span data-ttu-id="45d7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d7b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="45d7b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45d7b-124">Content-Type</span></span>  | <span data-ttu-id="45d7b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d7b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45d7b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45d7b-127">Request body</span></span>

<span data-ttu-id="45d7b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="45d7b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="45d7b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="45d7b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="45d7b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="45d7b-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="45d7b-131">Список свойств приведен в разделе [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="45d7b-131">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="45d7b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d7b-132">Response</span></span>

<span data-ttu-id="45d7b-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45d7b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45d7b-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="45d7b-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45d7b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="45d7b-136">Request</span></span>

<span data-ttu-id="45d7b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45d7b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45d7b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="45d7b-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="45d7b-139">C#</span><span class="sxs-lookup"><span data-stu-id="45d7b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45d7b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45d7b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45d7b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45d7b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45d7b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d7b-142">Response</span></span>

<span data-ttu-id="45d7b-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="45d7b-143">The following is an example of the response.</span></span>

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
