---
title: Обновление Кондитионалакцессполици
description: Обновление свойств объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 52d325f0a75bfdedf6ebf36d0a775efe9580739f
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062442"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="1b0ec-103">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="1b0ec-103">Update conditionalAccessPolicy</span></span>

<span data-ttu-id="1b0ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b0ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b0ec-105">Обновление свойств объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1b0ec-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b0ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0ec-106">Permissions</span></span>

<span data-ttu-id="1b0ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0ec-109">Permission type</span></span>                        | <span data-ttu-id="1b0ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b0ec-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="1b0ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b0ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b0ec-112">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b0ec-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="1b0ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b0ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b0ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-114">Not supported.</span></span> |
|<span data-ttu-id="1b0ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b0ec-115">Application</span></span>                            | <span data-ttu-id="1b0ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-116">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="1b0ec-117">У этого API есть [известная проблема](/graph/known-issues#permissions) , связанная с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="1b0ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b0ec-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b0ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b0ec-119">Request headers</span></span>

| <span data-ttu-id="1b0ec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b0ec-120">Name</span></span>          | <span data-ttu-id="1b0ec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1b0ec-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="1b0ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b0ec-122">Authorization</span></span> | <span data-ttu-id="1b0ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1b0ec-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b0ec-125">Content-Type</span></span>  | <span data-ttu-id="1b0ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b0ec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b0ec-128">Request body</span></span>

<span data-ttu-id="1b0ec-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1b0ec-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1b0ec-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="1b0ec-132">Список свойств приведен в разделе [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b0ec-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="1b0ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0ec-133">Response</span></span>

<span data-ttu-id="1b0ec-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b0ec-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="1b0ec-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b0ec-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b0ec-137">Request</span></span>

<span data-ttu-id="1b0ec-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b0ec-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b0ec-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
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
# <a name="c"></a>[<span data-ttu-id="1b0ec-140">C#</span><span class="sxs-lookup"><span data-stu-id="1b0ec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b0ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b0ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b0ec-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b0ec-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b0ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0ec-143">Response</span></span>

<span data-ttu-id="1b0ec-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1b0ec-144">The following is an example of the response.</span></span>

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
