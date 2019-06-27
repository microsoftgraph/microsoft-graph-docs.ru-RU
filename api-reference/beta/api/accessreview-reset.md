---
title: Сброс Акцессревиев
description: В средстве проверки доступа Azure AD выполните сброс решений текущего активного Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  Предыдущие решения не записываются, но проверяющие могут продолжать обновлять решения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e3f848b2e1c9d648ed0888bb30b72e2533f07eda
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258837"
---
# <a name="reset-accessreview"></a><span data-ttu-id="d4222-105">Сброс Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d4222-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4222-106">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD выполните сброс решений текущего активного [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="d4222-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="d4222-107">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="d4222-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="d4222-108">Предыдущие решения не записываются, но проверяющие могут продолжать обновлять решения.</span><span class="sxs-lookup"><span data-stu-id="d4222-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4222-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4222-109">Permissions</span></span>
<span data-ttu-id="d4222-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4222-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4222-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4222-112">Permission type</span></span>                        | <span data-ttu-id="d4222-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4222-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4222-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4222-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4222-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4222-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d4222-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4222-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4222-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4222-117">Not supported.</span></span> |
|<span data-ttu-id="d4222-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4222-118">Application</span></span>                            | <span data-ttu-id="d4222-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4222-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4222-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4222-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="d4222-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4222-121">Request headers</span></span>
| <span data-ttu-id="d4222-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d4222-122">Name</span></span>         | <span data-ttu-id="d4222-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d4222-123">Type</span></span>        | <span data-ttu-id="d4222-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d4222-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d4222-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4222-125">Authorization</span></span> | <span data-ttu-id="d4222-126">string</span><span class="sxs-lookup"><span data-stu-id="d4222-126">string</span></span> | <span data-ttu-id="d4222-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4222-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4222-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4222-129">Request body</span></span>
<span data-ttu-id="d4222-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4222-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d4222-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4222-131">Response</span></span>
<span data-ttu-id="d4222-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4222-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4222-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d4222-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4222-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4222-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
##### <a name="response"></a><span data-ttu-id="d4222-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4222-136">Response</span></span>
><span data-ttu-id="d4222-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4222-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4222-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d4222-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4222-140">C#</span><span class="sxs-lookup"><span data-stu-id="d4222-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reset_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4222-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4222-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reset_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d4222-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4222-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reset_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
