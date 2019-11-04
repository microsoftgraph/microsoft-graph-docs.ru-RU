---
title: Удаление Намедлокатион
description: Удаление объекта Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c5fb698736bf6c365f7956a3738e24f85ed479e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937983"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="6e589-103">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="6e589-103">Delete namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e589-104">Удаление объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="6e589-104">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e589-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e589-105">Permissions</span></span>

<span data-ttu-id="6e589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e589-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e589-108">Permission type</span></span>                        | <span data-ttu-id="6e589-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e589-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e589-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e589-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e589-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="6e589-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6e589-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e589-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e589-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e589-113">Not supported.</span></span> |
| <span data-ttu-id="6e589-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e589-114">Application</span></span>                            | <span data-ttu-id="6e589-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e589-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="6e589-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="6e589-116">This API requires multiple permissions.</span></span> <span data-ttu-id="6e589-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="6e589-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="6e589-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e589-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e589-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e589-119">Request headers</span></span>

| <span data-ttu-id="6e589-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6e589-120">Name</span></span>          | <span data-ttu-id="6e589-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6e589-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6e589-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e589-122">Authorization</span></span> | <span data-ttu-id="6e589-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e589-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e589-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e589-125">Request body</span></span>

<span data-ttu-id="6e589-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e589-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e589-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e589-127">Response</span></span>

<span data-ttu-id="6e589-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e589-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e589-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e589-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e589-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e589-131">Request</span></span>

<span data-ttu-id="6e589-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e589-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e589-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e589-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e589-134">C#</span><span class="sxs-lookup"><span data-stu-id="6e589-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e589-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e589-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e589-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e589-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e589-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e589-137">Response</span></span>

<span data-ttu-id="6e589-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6e589-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
