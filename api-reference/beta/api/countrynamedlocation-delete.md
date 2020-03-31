---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ea99659b8257a6d93ddd28fdc45f8221e78fecd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43061967"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="edec6-103">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="edec6-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="edec6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edec6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edec6-105">Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="edec6-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="edec6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edec6-106">Permissions</span></span>

<span data-ttu-id="edec6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="edec6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edec6-109">Permission type</span></span>                        | <span data-ttu-id="edec6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edec6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="edec6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edec6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="edec6-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="edec6-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="edec6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edec6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edec6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edec6-114">Not supported.</span></span> |
| <span data-ttu-id="edec6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edec6-115">Application</span></span>                            | <span data-ttu-id="edec6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edec6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edec6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edec6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="edec6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edec6-118">Request headers</span></span>

| <span data-ttu-id="edec6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="edec6-119">Name</span></span>          | <span data-ttu-id="edec6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="edec6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="edec6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edec6-121">Authorization</span></span> | <span data-ttu-id="edec6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edec6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edec6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edec6-124">Request body</span></span>

<span data-ttu-id="edec6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edec6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edec6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="edec6-126">Response</span></span>

<span data-ttu-id="edec6-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edec6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edec6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="edec6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edec6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="edec6-130">Request</span></span>

<span data-ttu-id="edec6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edec6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edec6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="edec6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="edec6-133">C#</span><span class="sxs-lookup"><span data-stu-id="edec6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edec6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edec6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edec6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edec6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="edec6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="edec6-136">Response</span></span>

<span data-ttu-id="edec6-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="edec6-137">The following is an example of the response.</span></span>

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
