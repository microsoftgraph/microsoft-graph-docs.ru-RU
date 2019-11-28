---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20b3058f46811edebe4fcf468f1156bf47971700
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636794"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="2f5aa-103">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="2f5aa-103">Delete countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f5aa-104">Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="2f5aa-104">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f5aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f5aa-105">Permissions</span></span>

<span data-ttu-id="2f5aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f5aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f5aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f5aa-108">Permission type</span></span>                        | <span data-ttu-id="2f5aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f5aa-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f5aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f5aa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f5aa-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="2f5aa-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="2f5aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f5aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f5aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-113">Not supported.</span></span> |
| <span data-ttu-id="2f5aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f5aa-114">Application</span></span>                            | <span data-ttu-id="2f5aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f5aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f5aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2f5aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f5aa-117">Request headers</span></span>

| <span data-ttu-id="2f5aa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2f5aa-118">Name</span></span>          | <span data-ttu-id="2f5aa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f5aa-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2f5aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f5aa-120">Authorization</span></span> | <span data-ttu-id="2f5aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f5aa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f5aa-123">Request body</span></span>

<span data-ttu-id="2f5aa-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f5aa-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f5aa-125">Response</span></span>

<span data-ttu-id="2f5aa-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f5aa-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f5aa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f5aa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f5aa-129">Request</span></span>

<span data-ttu-id="2f5aa-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f5aa-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f5aa-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f5aa-132">C#</span><span class="sxs-lookup"><span data-stu-id="2f5aa-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f5aa-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f5aa-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f5aa-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f5aa-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f5aa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f5aa-135">Response</span></span>

<span data-ttu-id="2f5aa-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f5aa-136">The following is an example of the response.</span></span>

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
