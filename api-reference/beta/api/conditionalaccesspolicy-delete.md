---
title: Удаление Кондитионалакцессполици
description: Удаление объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc4d00975fc92e9e561ebfaa1b403f351b0baf9d
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636773"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="15494-103">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="15494-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15494-104">Удаление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="15494-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="15494-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15494-105">Permissions</span></span>

<span data-ttu-id="15494-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15494-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15494-108">Permission type</span></span>                        | <span data-ttu-id="15494-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15494-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="15494-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15494-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15494-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="15494-111">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="15494-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15494-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15494-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15494-113">Not supported.</span></span> |
|<span data-ttu-id="15494-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15494-114">Application</span></span>                            | <span data-ttu-id="15494-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15494-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15494-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15494-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="15494-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15494-117">Request headers</span></span>

| <span data-ttu-id="15494-118">Имя</span><span class="sxs-lookup"><span data-stu-id="15494-118">Name</span></span>          | <span data-ttu-id="15494-119">Описание</span><span class="sxs-lookup"><span data-stu-id="15494-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="15494-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15494-120">Authorization</span></span> | <span data-ttu-id="15494-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15494-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15494-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15494-123">Request body</span></span>

<span data-ttu-id="15494-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15494-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15494-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="15494-125">Response</span></span>

<span data-ttu-id="15494-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15494-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15494-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="15494-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15494-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="15494-129">Request</span></span>

<span data-ttu-id="15494-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15494-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15494-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="15494-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15494-132">C#</span><span class="sxs-lookup"><span data-stu-id="15494-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15494-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15494-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15494-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15494-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15494-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="15494-135">Response</span></span>

<span data-ttu-id="15494-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15494-136">The following is an example of the response.</span></span>

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
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
