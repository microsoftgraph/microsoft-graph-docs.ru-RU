---
title: Удаление Кондитионалакцессполици
description: Удаление объекта Кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e8bc18b4608f08a8285c6b575e2ce96c204fc4
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916517"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="13b39-103">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="13b39-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="13b39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13b39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13b39-105">Удаление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="13b39-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13b39-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13b39-106">Permissions</span></span>

<span data-ttu-id="13b39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13b39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13b39-109">Permission type</span></span>                        | <span data-ttu-id="13b39-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13b39-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="13b39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13b39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13b39-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="13b39-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="13b39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13b39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13b39-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b39-114">Not supported.</span></span> |
|<span data-ttu-id="13b39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13b39-115">Application</span></span>                            | <span data-ttu-id="13b39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13b39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13b39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="13b39-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13b39-118">Request headers</span></span>

| <span data-ttu-id="13b39-119">Имя</span><span class="sxs-lookup"><span data-stu-id="13b39-119">Name</span></span>          | <span data-ttu-id="13b39-120">Описание</span><span class="sxs-lookup"><span data-stu-id="13b39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="13b39-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13b39-121">Authorization</span></span> | <span data-ttu-id="13b39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13b39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13b39-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13b39-124">Request body</span></span>

<span data-ttu-id="13b39-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13b39-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13b39-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="13b39-126">Response</span></span>

<span data-ttu-id="13b39-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13b39-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13b39-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="13b39-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13b39-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="13b39-130">Request</span></span>

<span data-ttu-id="13b39-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13b39-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13b39-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="13b39-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="13b39-133">C#</span><span class="sxs-lookup"><span data-stu-id="13b39-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13b39-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13b39-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13b39-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13b39-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13b39-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="13b39-136">Response</span></span>

<span data-ttu-id="13b39-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="13b39-137">The following is an example of the response.</span></span>

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
