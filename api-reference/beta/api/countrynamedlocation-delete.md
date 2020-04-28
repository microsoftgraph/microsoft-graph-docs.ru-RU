---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3043e1caa24ef7ad3da94b6a7cf5c3162f656ddd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375827"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="b305d-103">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="b305d-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="b305d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b305d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b305d-105">Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="b305d-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b305d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b305d-106">Permissions</span></span>

<span data-ttu-id="b305d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b305d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b305d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b305d-109">Permission type</span></span>                        | <span data-ttu-id="b305d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b305d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b305d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b305d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b305d-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b305d-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="b305d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b305d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b305d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b305d-114">Not supported.</span></span> |
| <span data-ttu-id="b305d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b305d-115">Application</span></span>                            | <span data-ttu-id="b305d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b305d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b305d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b305d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b305d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b305d-118">Request headers</span></span>

| <span data-ttu-id="b305d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b305d-119">Name</span></span>          | <span data-ttu-id="b305d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b305d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b305d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b305d-121">Authorization</span></span> | <span data-ttu-id="b305d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b305d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b305d-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b305d-124">Request body</span></span>

<span data-ttu-id="b305d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b305d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b305d-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="b305d-126">Response</span></span>

<span data-ttu-id="b305d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b305d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b305d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b305d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b305d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b305d-130">Request</span></span>

<span data-ttu-id="b305d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b305d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b305d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b305d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="b305d-133">C#</span><span class="sxs-lookup"><span data-stu-id="b305d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b305d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b305d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b305d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b305d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b305d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b305d-136">Response</span></span>

<span data-ttu-id="b305d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b305d-137">The following is an example of the response.</span></span>

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
  "description": "Delete countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
