---
title: 'Акцессревиевинстанце: АпплидеЦисионс'
description: Применение решений к Акцессревиевинстанце.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0af1ae1291a95145041a3e92bedf948c766bd1c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214771"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="c9b8c-103">Акцессревиевинстанце: АпплидеЦисионс</span><span class="sxs-lookup"><span data-stu-id="c9b8c-103">accessReviewInstance: applyDecisions</span></span>

<span data-ttu-id="c9b8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9b8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b8c-105">Применение решений по рецензированию для [акцессревиевинстанце](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="c9b8c-105">Apply review decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="c9b8c-106">Обратите внимание, что решения будут применяться автоматически, если параметр АутоапплидеЦисионсенаблед имеет значение true в [акцессревиевсчедулесеттингс](../resources/accessreviewschedulesettings.md)рецензирования.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-106">Note that decisions will be applied automatically if the autoApplyDecisionsEnabled parameter is True in the review's [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9b8c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b8c-107">Permissions</span></span>
<span data-ttu-id="c9b8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b8c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b8c-110">Permission type</span></span>                        | <span data-ttu-id="c9b8c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9b8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9b8c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9b8c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9b8c-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b8c-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c9b8c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9b8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b8c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-115">Not supported.</span></span>|
|<span data-ttu-id="c9b8c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c9b8c-116">Application</span></span>                            | <span data-ttu-id="c9b8c-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b8c-117">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9b8c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9b8c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="c9b8c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9b8c-119">Request headers</span></span>
|<span data-ttu-id="c9b8c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c9b8c-120">Name</span></span>|<span data-ttu-id="c9b8c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c9b8c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9b8c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9b8c-122">Authorization</span></span>|<span data-ttu-id="c9b8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c9b8c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9b8c-125">Content-Type</span></span>|<span data-ttu-id="c9b8c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b8c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9b8c-128">Request body</span></span>
<span data-ttu-id="c9b8c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9b8c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b8c-130">Response</span></span>
<span data-ttu-id="c9b8c-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c9b8c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9b8c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9b8c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9b8c-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c9b8c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9b8c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="c9b8c-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9b8c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-applydecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9b8c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9b8c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-applydecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9b8c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9b8c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-applydecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9b8c-138">Java</span><span class="sxs-lookup"><span data-stu-id="c9b8c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-applydecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c9b8c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b8c-139">Response</span></span>
<span data-ttu-id="c9b8c-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9b8c-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
