---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: aa7ceefca5201930f97d5e7befb6a7cc43c5715a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637600"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="00c6a-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="00c6a-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00c6a-104">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="00c6a-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00c6a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00c6a-105">Permissions</span></span>

<span data-ttu-id="00c6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00c6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00c6a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00c6a-108">Permission type</span></span>                        | <span data-ttu-id="00c6a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00c6a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="00c6a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00c6a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="00c6a-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="00c6a-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="00c6a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00c6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00c6a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00c6a-113">Not supported.</span></span> |
| <span data-ttu-id="00c6a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00c6a-114">Application</span></span>                            | <span data-ttu-id="00c6a-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="00c6a-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="00c6a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00c6a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="00c6a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00c6a-117">Request headers</span></span>

| <span data-ttu-id="00c6a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="00c6a-118">Name</span></span>          | <span data-ttu-id="00c6a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="00c6a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="00c6a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00c6a-120">Authorization</span></span> | <span data-ttu-id="00c6a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="00c6a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00c6a-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00c6a-122">Request body</span></span>

<span data-ttu-id="00c6a-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00c6a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00c6a-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="00c6a-124">Response</span></span>

<span data-ttu-id="00c6a-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="00c6a-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00c6a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="00c6a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00c6a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="00c6a-128">Request</span></span>

<span data-ttu-id="00c6a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00c6a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="00c6a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="00c6a-130">Response</span></span>

<span data-ttu-id="00c6a-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00c6a-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00c6a-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="00c6a-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00c6a-133">Языках</span><span class="sxs-lookup"><span data-stu-id="00c6a-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00c6a-134">Язык</span><span class="sxs-lookup"><span data-stu-id="00c6a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
