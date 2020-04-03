---
title: Остановить Акцессревиев
description: В функции рецензирования Access Azure AD остановите текущую активную Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  (Чтобы не допустить запуск последующих экземпляров проверки доступа, обновите его, чтобы изменить запланированную дату окончания).  После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c07cbb59d1c5411d6af27be919a18c15789acd97
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123372"
---
# <a name="stop-accessreview"></a><span data-ttu-id="9e738-106">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="9e738-106">Stop accessReview</span></span>

<span data-ttu-id="9e738-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e738-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e738-108">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD остановите текущую активную [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="9e738-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="9e738-109">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="9e738-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="9e738-110">(Чтобы не допустить запуск последующих экземпляров проверки доступа, [обновите его](accessreview-update.md) , чтобы изменить запланированную дату окончания).</span><span class="sxs-lookup"><span data-stu-id="9e738-110">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="9e738-111">После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="9e738-111">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e738-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e738-112">Permissions</span></span>
<span data-ttu-id="9e738-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e738-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e738-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e738-115">Permission type</span></span>                        | <span data-ttu-id="9e738-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e738-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e738-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e738-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e738-118">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9e738-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9e738-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e738-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e738-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e738-120">Not supported.</span></span> |
|<span data-ttu-id="9e738-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e738-121">Application</span></span>                            | <span data-ttu-id="9e738-122">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="9e738-122">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9e738-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e738-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="9e738-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e738-124">Request headers</span></span>
| <span data-ttu-id="9e738-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9e738-125">Name</span></span>         | <span data-ttu-id="9e738-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9e738-126">Type</span></span>        | <span data-ttu-id="9e738-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9e738-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9e738-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e738-128">Authorization</span></span> | <span data-ttu-id="9e738-129">string</span><span class="sxs-lookup"><span data-stu-id="9e738-129">string</span></span> | <span data-ttu-id="9e738-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e738-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e738-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e738-132">Request body</span></span>
<span data-ttu-id="9e738-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e738-133">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9e738-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e738-134">Response</span></span>
<span data-ttu-id="9e738-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e738-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e738-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9e738-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e738-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e738-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9e738-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e738-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="c"></a>[<span data-ttu-id="9e738-140">C#</span><span class="sxs-lookup"><span data-stu-id="9e738-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e738-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e738-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e738-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e738-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e738-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e738-143">Response</span></span>
><span data-ttu-id="9e738-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e738-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
