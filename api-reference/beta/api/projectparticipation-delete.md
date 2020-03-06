---
title: Удаление ПрожектпартиЦипатион
description: Удаление объекта ПрожектпартиЦипатион из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 723385798068e12ae03e6cf48943034ee7c887de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454943"
---
# <a name="delete-projectparticipation"></a><span data-ttu-id="be9ab-103">Удаление ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="be9ab-103">Delete projectParticipation</span></span>

<span data-ttu-id="be9ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be9ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be9ab-105">Удаление объекта [прожектпартиЦипатион](../resources/projectparticipation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="be9ab-105">Delete a [projectParticipation](../resources/projectparticipation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be9ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be9ab-106">Permissions</span></span>

<span data-ttu-id="be9ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be9ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be9ab-109">Permission type</span></span>                        | <span data-ttu-id="be9ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be9ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be9ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be9ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be9ab-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="be9ab-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be9ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be9ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be9ab-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="be9ab-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be9ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be9ab-115">Application</span></span>                            | <span data-ttu-id="be9ab-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9ab-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="be9ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be9ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="be9ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be9ab-118">Request headers</span></span>

| <span data-ttu-id="be9ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="be9ab-119">Name</span></span>           |<span data-ttu-id="be9ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be9ab-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="be9ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be9ab-121">Authorization</span></span>  | <span data-ttu-id="be9ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be9ab-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="be9ab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be9ab-124">Content-Type</span></span>   | <span data-ttu-id="be9ab-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be9ab-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be9ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be9ab-127">Request body</span></span>

<span data-ttu-id="be9ab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be9ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be9ab-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="be9ab-129">Response</span></span>

<span data-ttu-id="be9ab-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="be9ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be9ab-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="be9ab-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be9ab-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="be9ab-133">Request</span></span>

<span data-ttu-id="be9ab-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be9ab-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be9ab-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="be9ab-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_projectparticipation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/projects/{id}
```
# <a name="c"></a>[<span data-ttu-id="be9ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="be9ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be9ab-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be9ab-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be9ab-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be9ab-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be9ab-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="be9ab-139">Response</span></span>

<span data-ttu-id="be9ab-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="be9ab-140">The following is an example of the response.</span></span>

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
  "description": "Delete projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
