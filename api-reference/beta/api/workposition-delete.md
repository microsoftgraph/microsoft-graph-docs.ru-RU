---
title: Удаление Воркпоситион
description: Удаление объекта Воркпоситион из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 809552f0601e65e8478ab8e3a040821e9be09764
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938108"
---
# <a name="delete-workposition"></a><span data-ttu-id="c204c-103">Удаление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="c204c-103">Delete workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c204c-104">Удаление определенного объекта [воркпоситион](../resources/workposition.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c204c-104">Delete a specific [workPosition](../resources/workposition.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c204c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c204c-105">Permissions</span></span>

<span data-ttu-id="c204c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c204c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c204c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c204c-108">Permission type</span></span>                        | <span data-ttu-id="c204c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c204c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c204c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c204c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c204c-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c204c-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c204c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c204c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c204c-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c204c-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c204c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c204c-114">Application</span></span>                            | <span data-ttu-id="c204c-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c204c-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="c204c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c204c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c204c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c204c-117">Request headers</span></span>

| <span data-ttu-id="c204c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c204c-118">Name</span></span>           |<span data-ttu-id="c204c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c204c-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c204c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c204c-120">Authorization</span></span>  | <span data-ttu-id="c204c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c204c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c204c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c204c-123">Content-Type</span></span>   | <span data-ttu-id="c204c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c204c-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c204c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c204c-126">Request body</span></span>

<span data-ttu-id="c204c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c204c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c204c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c204c-128">Response</span></span>

<span data-ttu-id="c204c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c204c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c204c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c204c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c204c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c204c-132">Request</span></span>

<span data-ttu-id="c204c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c204c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_workposition"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/positions/{id}
```

### <a name="response"></a><span data-ttu-id="c204c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c204c-134">Response</span></span>

<span data-ttu-id="c204c-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c204c-135">The following is an example of the response.</span></span>

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
  "description": "Delete workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->