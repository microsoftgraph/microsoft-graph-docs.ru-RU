---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e7b7534031d392ff40379e87104ccd9dea3e8c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937171"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="4b925-103">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4b925-103">Delete countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b925-104">Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b925-104">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b925-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b925-105">Permissions</span></span>

<span data-ttu-id="4b925-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b925-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b925-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b925-108">Permission type</span></span>                        | <span data-ttu-id="4b925-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b925-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b925-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b925-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b925-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="4b925-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4b925-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b925-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b925-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b925-113">Not supported.</span></span> |
| <span data-ttu-id="4b925-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b925-114">Application</span></span>                            | <span data-ttu-id="4b925-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b925-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="4b925-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="4b925-116">This API requires multiple permissions.</span></span> <span data-ttu-id="4b925-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="4b925-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="4b925-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b925-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b925-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b925-119">Request headers</span></span>

| <span data-ttu-id="4b925-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4b925-120">Name</span></span>          | <span data-ttu-id="4b925-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4b925-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b925-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b925-122">Authorization</span></span> | <span data-ttu-id="4b925-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b925-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b925-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b925-125">Request body</span></span>

<span data-ttu-id="4b925-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b925-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b925-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b925-127">Response</span></span>

<span data-ttu-id="4b925-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b925-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b925-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b925-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b925-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b925-131">Request</span></span>

<span data-ttu-id="4b925-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b925-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b925-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b925-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b925-134">C#</span><span class="sxs-lookup"><span data-stu-id="4b925-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b925-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b925-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b925-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b925-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b925-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b925-137">Response</span></span>

<span data-ttu-id="4b925-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b925-138">The following is an example of the response.</span></span>

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
