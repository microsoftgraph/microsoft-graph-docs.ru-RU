---
title: Остановить Акцессревиев
description: В функции рецензирования Access Azure AD остановите текущую активную Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  (Чтобы не допустить запуск последующих экземпляров проверки доступа, обновите его, чтобы изменить запланированную дату окончания).  После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d919c42a5817b7c33dbc51fcc8c46fd4f443e067
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655392"
---
# <a name="stop-accessreview"></a><span data-ttu-id="89da7-106">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="89da7-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89da7-107">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD остановите текущую активную [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="89da7-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="89da7-108">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="89da7-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="89da7-109">(Чтобы не допустить запуск последующих экземпляров проверки доступа, обновите [его](accessreview-update.md) , чтобы изменить запланированную дату окончания).</span><span class="sxs-lookup"><span data-stu-id="89da7-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="89da7-110">После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="89da7-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="89da7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89da7-111">Permissions</span></span>
<span data-ttu-id="89da7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89da7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89da7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89da7-114">Permission type</span></span>                        | <span data-ttu-id="89da7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89da7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="89da7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89da7-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="89da7-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89da7-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="89da7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89da7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89da7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89da7-119">Not supported.</span></span> |
|<span data-ttu-id="89da7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89da7-120">Application</span></span>                            | <span data-ttu-id="89da7-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89da7-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="89da7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89da7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="89da7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89da7-123">Request headers</span></span>
| <span data-ttu-id="89da7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="89da7-124">Name</span></span>         | <span data-ttu-id="89da7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="89da7-125">Type</span></span>        | <span data-ttu-id="89da7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="89da7-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="89da7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="89da7-127">Authorization</span></span> | <span data-ttu-id="89da7-128">string</span><span class="sxs-lookup"><span data-stu-id="89da7-128">string</span></span> | <span data-ttu-id="89da7-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89da7-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89da7-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89da7-131">Request body</span></span>
<span data-ttu-id="89da7-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89da7-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="89da7-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="89da7-133">Response</span></span>
<span data-ttu-id="89da7-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89da7-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89da7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="89da7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89da7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="89da7-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
##### <a name="response"></a><span data-ttu-id="89da7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="89da7-138">Response</span></span>
><span data-ttu-id="89da7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89da7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="89da7-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="89da7-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89da7-142">C#</span><span class="sxs-lookup"><span data-stu-id="89da7-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/stop_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89da7-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="89da7-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/stop_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
