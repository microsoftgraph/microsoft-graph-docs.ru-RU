---
title: Обновление Кондитионалакцессполици
description: Обновление свойств объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c290faff53b98e28dc9876b9fd76abac8a813196
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936723"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="73427-103">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="73427-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73427-104">Обновление свойств объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="73427-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73427-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73427-105">Permissions</span></span>

<span data-ttu-id="73427-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73427-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73427-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73427-108">Permission type</span></span>                        | <span data-ttu-id="73427-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73427-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="73427-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73427-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73427-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="73427-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="73427-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73427-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73427-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73427-113">Not supported.</span></span> |
|<span data-ttu-id="73427-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73427-114">Application</span></span>                            | <span data-ttu-id="73427-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73427-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="73427-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="73427-116">This API requires multiple permissions.</span></span> <span data-ttu-id="73427-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="73427-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="73427-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73427-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73427-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73427-119">Request headers</span></span>

| <span data-ttu-id="73427-120">Имя</span><span class="sxs-lookup"><span data-stu-id="73427-120">Name</span></span>          | <span data-ttu-id="73427-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73427-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="73427-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73427-122">Authorization</span></span> | <span data-ttu-id="73427-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73427-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="73427-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73427-125">Content-Type</span></span>  | <span data-ttu-id="73427-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73427-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73427-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73427-128">Request body</span></span>

<span data-ttu-id="73427-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="73427-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="73427-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="73427-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73427-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="73427-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="73427-132">Список свойств приведен в разделе [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="73427-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="73427-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="73427-133">Response</span></span>

<span data-ttu-id="73427-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73427-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73427-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="73427-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73427-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="73427-137">Request</span></span>

<span data-ttu-id="73427-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73427-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73427-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="73427-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="73427-140">C#</span><span class="sxs-lookup"><span data-stu-id="73427-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73427-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73427-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73427-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73427-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73427-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="73427-143">Response</span></span>

<span data-ttu-id="73427-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73427-144">The following is an example of the response.</span></span>

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
