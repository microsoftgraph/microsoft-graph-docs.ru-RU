---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e7a1f3af86ec603c360d66d1b3c9d757d1da2254
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270730"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="f758c-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="f758c-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f758c-104">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="f758c-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f758c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f758c-105">Permissions</span></span>

<span data-ttu-id="f758c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f758c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f758c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f758c-108">Permission type</span></span>                        | <span data-ttu-id="f758c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f758c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f758c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f758c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f758c-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f758c-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="f758c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f758c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f758c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f758c-113">Not supported.</span></span> |
| <span data-ttu-id="f758c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f758c-114">Application</span></span>                            | <span data-ttu-id="f758c-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f758c-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f758c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f758c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f758c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f758c-117">Request headers</span></span>

| <span data-ttu-id="f758c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f758c-118">Name</span></span>          | <span data-ttu-id="f758c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f758c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f758c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f758c-120">Authorization</span></span> | <span data-ttu-id="f758c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f758c-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f758c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f758c-122">Request body</span></span>

<span data-ttu-id="f758c-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f758c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f758c-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="f758c-124">Response</span></span>

<span data-ttu-id="f758c-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f758c-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f758c-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="f758c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f758c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f758c-128">Request</span></span>

<span data-ttu-id="f758c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f758c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="f758c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f758c-130">Response</span></span>

<span data-ttu-id="f758c-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f758c-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f758c-132">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f758c-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f758c-133">C#</span><span class="sxs-lookup"><span data-stu-id="f758c-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f758c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f758c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f758c-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f758c-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
