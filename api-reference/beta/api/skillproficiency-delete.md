---
title: Удаление СкиллпрофиЦиенци
description: Удаление СкиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 06750de56dfa32ae5f339baacfc313360b0e973a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937611"
---
# <a name="delete-skillproficiency"></a><span data-ttu-id="76e30-103">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="76e30-103">Delete skillProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76e30-104">Удаление объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="76e30-104">Delete a [skillProficiency](../resources/skillproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76e30-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76e30-105">Permissions</span></span>

<span data-ttu-id="76e30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76e30-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76e30-108">Permission type</span></span>                        | <span data-ttu-id="76e30-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76e30-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76e30-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76e30-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="76e30-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="76e30-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="76e30-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76e30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e30-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="76e30-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="76e30-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76e30-114">Application</span></span>                            | <span data-ttu-id="76e30-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e30-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="76e30-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76e30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76e30-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76e30-117">Request headers</span></span>

| <span data-ttu-id="76e30-118">Имя</span><span class="sxs-lookup"><span data-stu-id="76e30-118">Name</span></span>           |<span data-ttu-id="76e30-119">Описание</span><span class="sxs-lookup"><span data-stu-id="76e30-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="76e30-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76e30-120">Authorization</span></span>  | <span data-ttu-id="76e30-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76e30-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="76e30-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76e30-123">Content-Type</span></span>   | <span data-ttu-id="76e30-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76e30-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="76e30-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76e30-126">Request body</span></span>

<span data-ttu-id="76e30-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76e30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76e30-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="76e30-128">Response</span></span>

<span data-ttu-id="76e30-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="76e30-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76e30-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="76e30-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76e30-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="76e30-132">Request</span></span>

<span data-ttu-id="76e30-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76e30-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_skillproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/skills/{id}
```

### <a name="response"></a><span data-ttu-id="76e30-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="76e30-134">Response</span></span>

<span data-ttu-id="76e30-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76e30-135">The following is an example of the response.</span></span>

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
  "description": "Delete skillProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->